---
created: 2021-04-27
time: 09:39:13
tags: Share-and-Showcase
---

# Toying with Relational Databases using Dataview

Assuming a prerequisite knowledge of Relational Databases, for example the ones in Notion, we proceed to their implementation using the Dataview plugin. I am taking a toy example of a college hub to go though this process.

# Creating multiple Databases
In Obsidian Dataview, creating separate databases must be created through creating notes(or pages). Each page must be organised into a specific database, though some field, most appropriate might be a hash#tag, but to reduce clutter one may use a `category:` field.

> Here, Categories (each being a separate database or group of pages) 
= {Semester, Course, Person, Lecture, Readings, Tutorial, Test}

We start now creating typical pages for each category:

<table>
<thead>
  <tr>
    <th>Title: Semester 1</th>
    <th>Title: MAT101</th>
    <th>Title: Nikunj</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>category: semester<br><br># Semester 1 Courses<br><br>~~~dataview<br>Table subject, syllabus, teacher, teacher.mail<br>FROM ""<br>SORT semester<br>WHERE category="course" AND semester=[[Semester 1]]<br>~~~<br></td>
    <td>category:: course<br>semester:: [[Semester 1]]<br>subject:: [[MAT]]<br>syllabus:: [[a.pdf]]<br>teacher:: [[Nikunj]]<br><br><br>This course is taught by `= this.teacher`, available at `= this.teacher.mail`.<br></td>
    <td>mail:: nikunj@gmail.com</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
</tbody>
</table>

Which gives this as preview:
![](https://i.imgur.com/hB4Fnf3.png)
![](https://i.imgur.com/rXEZ8F6.png)

So we have already prepared a relational database connection with teacher and course.

# Proper creation of relation
Relation (for example Relation in Notion Databases) is not bidirectional in Dataview. Only in one of the pages the field+link can be made, and if the practice is not made properly, the database can break.

Proceeding with an example, let's consider our course MAT101 has some lectures attached to it.

File: [[MAT101.L01]]
```
category:: lecture
course:: [[MAT101]]
date:: @23MAY21
```

And each lecture has some pre-lecture reading and post-lecture tutorials. I will make this two connection in two ways that it can be made.

File: [[MAT101.R01]]
```
category:: reading
lecture:: [[MAT101.L01]]
material:: [[Matter.pdf]]
```

File: [[MAT101.L01]] ~ changes made from above
```
category:: lecture
course:: [[MAT101]]
date:: @23MAY21
tutorials:: [[MAT101.T01]]
``` 

It is evident that the Readings page has field+link to the lecture(s) and the lecture pages themselves have the field+link to the tutorial pages. Lecture pages are higher in the hierarchy but the linking in done in two ways: reading->lecture and lecture->tutorial.

So, it can be now understood, all Readings pages must have the lecture field. It cannot be the other way around in the middle, a lecture having reading field. In Notion, this shows up bidirectionally. But here the field+link cannot be placed in both places automatically.


# Rollups

If the premise *one must follow the appropriate placement of field in all of the user defined-category pages continuously* we can have proper Dataview rollups, no matter the type connection we are making (the reading->lecture way or the lecture->tutorial way; where lectures are higher in the hierarchy)

Following examples gives the rollup of readings and tutorials with-respect-to the list of lectures.

For the reading->lecture rollup is a bit tricky, we make a table of *reading* files and group them by lectures. The lecture->tutorial rollup is fairly straightforward.

File: [[MAT101.L01]] ~ addition made after above
```
# Pre-Lecture Reading Material by Lectures
~~~dataview
Table lecture,rows.file.link AS "readings", lecture.date, lecture.course.teacher
WHERE category="reading"
flatten lecture
group by lecture
~~~

# Post-Lecture Tutorials by Lectures

~~~dataview
Table tutorials
FROM ""
WHERE category="lecture"
~~~
```
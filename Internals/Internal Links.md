---
created: 2021-05-03
time: 14:39:22
tags:
---

# Internal Links

%%
# Link emojis (plugin)
- Is not working yet

[mdelobelle/obsidian_supercharged_links: obsidian plugin to add attributes to internal links](https://github.com/mdelobelle/obsidian_supercharged_links)

#CSS
```css
a.internal-link[category="people"]{
    text-decoration: none;
    background-color: grey;
    color: white;
    padding: 3px 12px;
    border-radius: 15px
}

a.internal-link[category="people"]::before {
    content: "👤 "
}

a.internal-link[next-action="call"]::after {
    content: " > ☎️"
}
```

%%
---
tags:
  - topics
---

```dataview
table without id
	file.link as Show,
	rating as Rating, 
	last as "Last seen"
where
	contains(topics, this.file.link) and
	!contains(file.name, "Template")
sort last desc
```


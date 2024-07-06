---
tags:
  - topics
---
## Places


```dataview
table without id
	file.link as Place,
	loc as Location,
	type as Type,
	rating as Rating
where
	contains(topics,this.file.link) and
	!contains(file.tags,"places/types") and
	!contains(file.name,"Template") and
	!contains(type, "[[City]]")
sort type asc
```


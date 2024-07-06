---
tags:
  - topics
---
```dataview
table without id
	file.link as Title,
	status as Status,
	published as Published
where
	contains(topics,this.file.link) and
	!contains(file.name,"Template")
sort published desc
```

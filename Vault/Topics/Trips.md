---
tags:
  - topics
---

```dataview
table without id
	file.link as Trip,
	loc as Location,
	start as Start,
	end as End
where
	contains(topics,[[Trips]]) and
	!contains(file.name, "Template") and
	!contains(file.name, "Planning")
sort start desc
```


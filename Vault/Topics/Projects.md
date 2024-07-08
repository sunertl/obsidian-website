---
tags:
  - topics
---

```dataview
table 
	type as Type,
	year as Year,
	status as Status
where
	contains(topics,[[Projects]]) and
	!contains(file.name,"Template")
sort year desc
```


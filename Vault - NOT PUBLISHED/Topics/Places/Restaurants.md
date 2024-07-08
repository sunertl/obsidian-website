---
tags:
  - food
---
```dataview
table without id
	file.link as "List of Restaurants",
	loc as "Location",
	rating as "Rating"
	from -"Meta/Templates"
where contains(type, [[Restaurants]]) and
last != "" and !contains(file.name, "Template")
sort file.name ASC
limit 50
```




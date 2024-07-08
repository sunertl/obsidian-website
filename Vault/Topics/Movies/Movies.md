---
tags:
  - topics
---
## Favorites

```dataview
table without id
	file.link as Movie,
	year as Year,
	rating as Rating,
	last as "Last seen",
	director as Director
where
	contains(topics,this.file.link)
	and rating > 8
sort rating desc
```

## Last seen

```dataview
table without id
	file.link as Movie,
	year as Year,
	rating as Rating,
	last as "Last seen",
	director as Director
where
	contains(topics,this.file.link) and
	!contains(file.name, "Template")
sort last desc
limit 150
```


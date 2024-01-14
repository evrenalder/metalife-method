---
weight:
---

# <% tp.file.title %>

---

<< [[<% tp.date.yesterday("YYYY-MM-DD") %>]] | [[Template - Daily Note]] | [[<% tp.date.tomorrow("YYYY-MM-DD") %>]] >>

---
## To Do List

```dataviewjs
dv.table([
	"Name",   
	"Due",
	"Ext Tracking"
	],
	dv.pages("#type/task")
    	.sort(t => [ t.rank, t.due ], 'asc')
		.where(t => 
			!t.completed &&
			t.file.path.includes('2 Areas/Tasks/Tasks-Open')
		)
		.limit(5)
		.map(t => 
			[
				t.file.link, 
				t.due,
				t.externalTrackingId
			])
    )
```

**[[🔘 TASKS DB]] | [[2 Areas/Tasks/TASKS DV TABLE]]**

---
## Doing / Done

*Today's Headings and Notes...*


## A more sophisticated example using a Dataview JS query

```dataviewjs
dv.table([
	"Name",   
	"Due",
	"External Tracking ID"
	],
	dv.pages("#type/task")
    	.sort(t => [ t.rank, t.due ], 'asc')
		.where(t => 
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

This task list is created with the following Dataview JS query:

````
```dataviewjs
dv.table([
	"Name",   
	"Due",
	"External Tracking ID"
	],
	dv.pages("#type/task")
    	.sort(t => [ t.rank, t.due ], 'asc')
		.where(t => 
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
````


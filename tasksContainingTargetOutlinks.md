---
who: [[[person1]], [[person2]]]
```
## Tasks

- [ ] Task for [[person1]]
- [ ] Task for [[person2]]
- [x] Task for [[person1]]

## Query
```dataviewjs
const groupByFile = false; // should dv.taskList be grouped by file?

function tasksContainingTargetOutlinks(){

	//get array with all oulinks contained in target frontmatter 
	let targetOutlinks = new Array; 
	dv.current()["who"].forEach(t => targetOutlinks.push(t.path));
	
	//get all incomplete tasks with outlinks
	let tasks = dv.pages().file.tasks
		.where(t => t.outlinks.length > 0 && !t.completed)
		.filter(t => t.outlinks.every(o => targetOutlinks.includes(o.path)));

	return tasks;
}

// const intersection = array1.filter(element => array2.includes(element)); works for two arrays comparason but you need .every since tasks is an objecct and you want the path value from the outlinks key. 

//display
dv.taskList(tasksContainingTargetOutlinks(), groupByFile);
```

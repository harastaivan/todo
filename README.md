# todo
todo list for terminal

## usage

- [ ] `todo init` initializes new todo list (creates `.todo.json` file in home directory)
- [ ] `todo list` lists all todos
- [ ] `todo add proj some text of the todo` creates new todo in project `proj`
- [ ] `todo edit 5 project proj2` changes todo with id 5 project to `proj2`
- [ ] `todo edit 5 text new text for the todo` changes todo with id 5 text
- [ ] `todo complete 5` completes todo with id 5
- [ ] `todo delete 5` deletes todo with id 5
- [ ] `todo spend 5 1h 30m` increases spent time on todo 5 by 1 hour and 30 minutes
- [ ] `todo history` show history of changes
- [ ] `todo back` reverts last change (can be used repeatedly)

### init

```
$ todo init
New todo list initialized (.todo.json)
```

### add

```
$ todo add work implement a feature
New todo implement a feature added to work project
$ todo add school learn an exam
New todo learn an exam added to school project
```

### list

```
$ todo list
school
[ ] 2 0h 0m learn an exam
work
[ ] 1 0h 0m implement a feature
```

### spend, complete

```
$ todo spend 2 1h 40m
[ ] 2 1h 40m learn an exam
$ todo complete 2
[x] 2 1h 40m learn an exam
$ todo list
school
[x] 2 1h 40m learn an exam
work
[ ] 1 0h 0m implement a feature
```

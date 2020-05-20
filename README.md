
# To do format

This is a newish format for tracking task lists in plain text format.

Using this format you can keep track of your daily tasks and keep a complete
log of everything you've done.

Here's a short example:

```
Wed 20 May
[ ] do this task today
[v] this task is done
[ ] this is an open task with sub-tasks
	- for example this one
	v this one is completed
	- this one is not
``` 


# Highlighter

This repo includes a syntax file for Sublime Text 3 which, when used with
the Monokai theme, nicely highlights items and greyes out completed task
in a way that makes it easy to see the state of your task list at a glance.


# Questions

#### When not to use this

- if you are about support by other apps - there are none!

#### Why plain text?

- Compatible with all text editors
- Compatible with cloud solutions (dropbox, git)

#### Why not [todo.txt][todotxt]?

I found it not easily readable at a glance. Each task is confined to one line, there are no subtasks,
and the tasks, checkmarks and timestamps are all over the place. I preferred something
that looked like a bulleted list with checkboxes more than anything else, and I found
prioritizing items by starting lines with `(A)` or `(B)` unclear and unpractical.

This TODO approach also targets the average, quick, daily to-do list rather than
an issue tracker for projects. You list what you do today, without categorising
using tags, project names, due dates or priorities.

If you want to add priority to a task, simply move it to the top.

#### Why not Markdown?

Markdown checkboxes only allow for two states: done, or not done, and has no room for
'eh'. It also requires two more characters to add a checkbox: `- [*]`. Yuk!


# Complete definition

#### Task states

Tasks and subtasks alike can exist in several states:

- open  (`[ ]`)
- completed (`[v]`)
- canceled (`[x]`)
- may be canceled (`[?]`)
- may be canceled (`[~]`)

The first 3 speak for themselves, the other two indicate uncertainties. For example,
if you partially completed a task and are not sure enough if it is 'good enough' yet,
use the `~` tilde to change the color of the task to yellow: it's not greyed
out yet, it is highlighted so you can easily find it and go back to it.


#### Subtasks

The same goes for subtasks. With exception that they are shaped more like a bulleted
list (no `[` `]` brackets, and a `-` dash for open items), the state indicators
have the same effect.

When a main task is closed or highlighted, this effects the subtasks too.


#### Grouping lists

To make lists of lists, you can add titles and separators:

```
=== This is a title ===

A subtle separator (can be any length)

-----------------------

And a heavy separator:

=======================
```

#### Dates

Personally, I don't see this as due dates but rather as the dates on which you plan
to do something. Does 'clean the kitchen' have a due date? Not really, but if you have
time this Tuesday, that's when you schedule it. Here's an example workflow:

```
Tue 5
[ ] Clean the kitchen

Mon 4
[ ] Do a thing

Sun 3 April
[ ] make a list
[v] tick things off
```

#### Time

Again not a due time, but rather a time indication. "Package will be delivered between 15:00 and 18:00" will
look like this:

```
[ ] 15:00 - 18:00 Package delivery
```


# Installation instructions

The syntax highlighter is not in the Sublime package thing yet.

```
// TODO
```

# License

```
Copyright © 2020 Mathijs Lagerberg
This work is free. You can redistribute it and/or modify it under the
terms of the Do What The Fuck You Want To Public License, Version 2,
as published by Sam Hocevar. See the COPYING file for more details.
```


[todotxt]: https://github.com/todotxt/todo.txt

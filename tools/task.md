# task

## Default task

If you execute `task` without any parameters it will look for a task named 
"default".

## Watch tasks

Somewhat hidden is the ability for task to make every task watchable.

Once a task has the keys `sources` and `generates` you can simply watch it by
adding `--watch`  or `-w` to the execution. To watch the default task for
example you would run `task -w`.

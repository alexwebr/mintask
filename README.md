mintask
=======

Simple todo list functionality for Vim.

To Use
-----
Just append the code in `mintask` to you `.vimrc` file.

This is what a mintask todo list can look like:

```
Alex's Todo List
 [ ] Prepare for Las Vegas
    [ ] Put clothes together
       [ ] Find good duffel
       [+] Buy more shorts
    [+] Figure out about hotel
    [+] Research carry-on sizes
 [ ] Install AIX 6 
   >[ ] Get NIM configured
    [+] Download AIX installation material - Thu Jul 19 14:09:23 CDT 2012
    [+] Patch lpp_source
 [ ] Patches for Nmap script
    [ ] Refactor arrow code
   >[ ] Get root directory scriptarg working
```

Tutorial
---------
mintask has two kinds of tasks - tasks, and subtasks.

All mintask commands are two characters, and are prefixed with a lowercase `t` (except for `T`, which jumps between all top-level tasks)

_New_ tasks are created with `tn`. _Sub_ tasks are created by putting your cursor over a task (or subtask) and typing `ts`. Tasks (and subtasks) are automatically marked as incomplete when they have a subtask added to them.

You can _mark_ one or more tasks (what that means is up to you) by putting your cursor on a task and typing `tm`. To remove a mark, type `tM`

You can mark a task as _complete_ by moving your cursor to it and typing `tc`. You can undo this with `tC`.

You can mark a task as complete and give it a _timestamp_ with `tt` - you can undo that with `tT`

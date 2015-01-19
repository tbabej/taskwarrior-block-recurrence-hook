Taskwarrior Block Recurrence Hook
-------------------------------------------

This is a hook for TaskWarrior (http://www.taskwarrior.org),
which blocks spawning of child recurrence tasks on the client where
it is enabled.

This is useful as a workaround for https://bug.tasktools.org/browse/TD-44
where different clients would spawn different child recurrence tasks for
the same parent task.

Install
-------

```
git clone https://github.com/tbabej/taskwarrior-block-recurrence-hook.git
cp taskwarrior-block-recurrencehook/on-* ~/.task/hooks/
```

This hook leverages tasklib, so you need to install that too:

```
pip install tasklib
```

Example of usage
----------------

Put into your .task/hooks folder and observe that recurrent tasks
are not being generated.

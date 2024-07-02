Thus far, you learned how to run simple shell commands like echo "Something" via run: echo "Something".

If you need to run multiple shell commands (or multi-line commands, e.g., for readability), you can easily do so by adding the pipe symbol (|) as a value after the run: key.

Like this:
```
...
run: |
    echo "First output"
    echo "Second output"
```
This will run both commands in one step.

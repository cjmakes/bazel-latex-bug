bazel-latex-bug
===============
bazel-latex rules fail when `spawn_strategy` is set to local. This is a minimal repoduction of the bug. Expose bug with:
```
# Does not work
bazel build --spawn_strategy=local ...

# Works
bazel build --spawn_strategy=sandboxed ...
```

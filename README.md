# Reproduce the error with

```bash
# Generate requirements_lock.txt
bazel run //tools/python_requirements:requirements.update
# Run python binary
bazel run //src:hello_world
```

The error I get running these commands
```
INFO: Running command line: bazel-bin/src/hello_world
Traceback (most recent call last):
  File "/home/bechir.braham/.cache/bazel/_bazel_bechir.braham/19aa4ce07a498ac9f4d24e6ab399522b/execroot/_main/bazel-out/k8-fastbuild/bin/src/hello_world.runfiles/_main/src/hello_world.py", line 2, in <module>
    import torch_tensorrt
ModuleNotFoundError: No module named 'torch_tensorrt'
```

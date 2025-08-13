# Reproduce the error with

```bash
# Generate requirements_lock.txt
bazel run //tools/python_requirements:requirements.update
# Run python binary
bazel run //src:hello_world
```

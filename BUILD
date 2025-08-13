load("//tools:requirements.bzl", "pip_requirements")

pip_requirements(
    name = "requirements_lock",
    requirements_in = "//src:requirements.in",
)

py_binary(
    name = "main",
    srcs = ["//src:main.py"],
    deps = ["@pip_deps//:cowsay"],
)

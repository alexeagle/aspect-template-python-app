load("@rules_uv//uv:pip.bzl", "pip_compile")

filegroup(
    name = "requirements",
    srcs = ["requirements.txt"],
    visibility = ["//requirements:__pkg__"],
)

pip_compile(
    name = "pip_compile",
    requirements_in = "pyproject.toml",
    requirements_txt = "requirements.txt",
    visibility = ["//requirements:__pkg__"],
)

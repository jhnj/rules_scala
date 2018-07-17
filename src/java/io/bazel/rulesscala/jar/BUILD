java_library(
    name = "jar",
    javacopts = [
        "-source 1.8",
        "-target 1.8",
    ],
    srcs = [
        "JarCreator.java",
        "JarHelper.java",
    ],
    visibility = ["//visibility:public"],
)

java_binary(
    name = "binary",
    javacopts = [
        "-source 1.8",
        "-target 1.8",
    ],
    main_class = "io.bazel.rulesscala.jar.JarCreator",
    visibility = ["//visibility:public"],
    runtime_deps = [
        ":jar",
    ],
)

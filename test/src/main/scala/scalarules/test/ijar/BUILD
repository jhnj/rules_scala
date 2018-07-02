package(default_visibility = ["//visibility:public"])

load("@io_bazel_rules_scala//scala:scala.bzl", "scala_library", "scala_test", "scala_binary")

scala_library(
    name = "user",
    srcs = [
        "A.scala",
    ],
    deps = ["dependency"],
)

scala_library(
    name = "dependency",
    srcs = [
        "B.scala",
        "C.java",
    ],
)

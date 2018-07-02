load("@io_bazel_rules_scala//scala:scala.bzl", "scala_binary")

scala_binary(
    name = "classpath_resource",
    srcs = ["ObjectWithClasspathResources.scala"],
    classpath_resources = [
        "//src/main/resources/scalarules/test:byes",
        "//src/main/resources/scalarules/test:hellos",
        "//src/main/resources/scalarules/test:more-byes",
        "//src/main/resources/scalarules/test:more-hellos",
    ],
    main_class = "scalarules.test.classpathresources.ObjectWithClasspathResources",
    visibility = ["//visibility:public"],
)

scala_binary(
    name = "classpath_resource_duplicates",
    srcs = ["ObjectWithDuplicateClasspathResources.scala"],
    classpath_resources = [
        "//src/main/resources/scalarules/test/classpath_resource1:classpath-resource",
        "//src/main/resources/scalarules/test/classpath_resource2:classpath-resource",
    ],
    main_class = "scalarules.test.classpathresources.ObjectWithDuplicateClasspathResources",
)

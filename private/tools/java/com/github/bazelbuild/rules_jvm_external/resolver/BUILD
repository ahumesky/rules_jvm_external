load("@rules_java//java:defs.bzl", "java_library")
load("//private/rules:artifact.bzl", "artifact")

java_library(
    name = "resolver",
    srcs = glob(["*.java"]),
    visibility = [
        "//private/tools/java:__subpackages__",
        "//tests/com/github/bazelbuild/rules_jvm_external:__subpackages__",
    ],
    deps = [
        "//private/tools/java/com/github/bazelbuild/rules_jvm_external",
        artifact(
            "com.google.guava:guava",
            repository_name = "rules_jvm_external_deps",
        ),
    ],
)

package(default_visibility = ["//visibility:public"])

load("@rules_antlr//antlr:antlr3.bzl", "antlr3")

antlr3(
    name = "generated",
    srcs = glob(["src/main/antlr3/*.g"]),
)

java_library(
    name = "InheritSameFolder",
    srcs = [":generated"],
    deps = ["@antlr3_runtime//jar"],
)

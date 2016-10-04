package(default_visibility = ["//visibility:public"])

load("@org_pubref_rules_protobuf//java:rules.bzl", "java_proto_library")

java_proto_library(
    name = "java",
    protos = ["common.proto"],
    imports = ['external/com_github_google_protobuf/src'],
    verbose = 1,
)

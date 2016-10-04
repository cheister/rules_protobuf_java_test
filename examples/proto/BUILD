package(default_visibility = ["//visibility:public"])

load("@org_pubref_rules_protobuf//java:rules.bzl", "java_proto_library")

java_proto_library(
    name = "wkt_protos",
    protos = ["@com_github_google_protobuf//:well_known_protos"],
    imports = ['external/com_github_google_protobuf/src'],
)

java_proto_library(
    name = "java",
    protos = ["common.proto"],
    proto_deps = [
        "wkt_protos",
    ],
    imports = ['external/com_github_google_protobuf/src'],
    inputs = ["@com_github_google_protobuf//:well_known_protos"],
    verbose = 2,
)

licenses(["notice"])
package(default_visibility = ["//visibility:public"])

load("@org_pubref_rules_protobuf//java:rules.bzl", "java_proto_library")

java_proto_library(
    name = "google_well_known_protos",
    protos = ["@com_github_google_protobuf//:well_known_protos"],
    imports = ['src'],
)

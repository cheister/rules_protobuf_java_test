package(default_visibility = ["//visibility:public"])

load("@org_pubref_rules_protobuf//java:rules.bzl", "java_proto_library")

java_proto_library(
    name = "google_well_known_protos",
    protos = ["@com_github_google_protobuf//:well_known_protos"],
    imports = ['src'],
)

java_proto_library(
    name = "common_proto_java",
    protos = ["common.proto"],
    proto_deps = ["google_well_known_protos"],
    imports = ["external/com_github_google_protobuf/src"],
    inputs = ["@com_github_google_protobuf//:well_known_protos"],
    verbose = 2,
)

java_proto_library(
  name = 'common_proto_java_with_third_party_dep',
  deps = [
     '//third_party/protobuf:google_well_known_protos',
  ],
  protos = ["common.proto"],
  imports = ['external/com_github_google_protobuf/src'],
  verbose = 2,
)

package(default_visibility = ["//visibility:public"])

licenses(["notice"])

proto_library(
    name = "semver_proto",
    srcs = ["semver.proto"],
    proto_source_root = package_name(),
)

java_proto_library(
    name = "semver_java_proto",
    deps = [":semver_proto"],
)


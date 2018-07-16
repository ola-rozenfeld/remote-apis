workspace(name = "bazel_remote_apis")

# Java gRPC library.
http_archive(
    name = "grpc_java",
    sha256 = "df39e0fbdf5f8260c6b369dc240e5d0956d804588eaa15fe46e20c7a589f2163",
    strip_prefix = "grpc-java-1.10.0",
    urls = [
        "https://github.com/grpc/grpc-java/archive/v1.10.0.tar.gz",
    ],
)
load("@grpc_java//:repositories.bzl", "grpc_java_repositories")
grpc_java_repositories()

# Needed for the googleapis protos.
new_http_archive(
    name = "googleapis",
    build_file = "BUILD.googleapis",
    sha256 = "7b6ea252f0b8fb5cd722f45feb83e115b689909bbb6a393a873b6cbad4ceae1d",
    strip_prefix = "googleapis-143084a2624b6591ee1f9d23e7f5241856642f4d",
    url = "https://github.com/googleapis/googleapis/archive/143084a2624b6591ee1f9d23e7f5241856642f4d.zip",
)

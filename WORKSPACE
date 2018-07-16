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

#http_archive(
#      name = "io_grpc_grpc_java",
#      urls = [
#          "https://mirror.bazel.build/github.com/grpc/grpc/archive/v1.10.0.tar.gz",
#          "https://github.com/grpc/grpc/archive/v1.10.0.tar.gz",
#      ],
#      sha256 = "39a73de6fa2a03bdb9c43c89a4283e09880833b3c1976ef3ce3edf45c8cacf72",
#      strip_prefix = "grpc-1.10.0",
#    name = "io_grpc_grpc_java",
#    sha256 = "5ba69890c9fe7bf476093d8863f26b861184c623ba43b70ef938a190cfb95bdc",
#    strip_prefix = "grpc-java-1.12.0",
#    urls = [
#        "https://github.com/grpc/grpc-java/archive/v1.12.0.tar.gz",
#    ],
#)

## Needed for "well-known protos" and protoc.
#http_archive(
#    name = "com_google_protobuf",
#    sha256 = "091d4263d9a55eccb6d3c8abde55c26eaaa933dea9ecabb185cdf3795f9b5ca2",
#    strip_prefix = "protobuf-3.5.1.1",
#    urls = ["https://github.com/google/protobuf/archive/v3.5.1.1.zip"],
#)

# Needed for the googleapis protos.
new_http_archive(
    name = "googleapis",
    build_file = "BUILD.googleapis",
    sha256 = "7b6ea252f0b8fb5cd722f45feb83e115b689909bbb6a393a873b6cbad4ceae1d",
    strip_prefix = "googleapis-143084a2624b6591ee1f9d23e7f5241856642f4d",
    url = "https://github.com/googleapis/googleapis/archive/143084a2624b6591ee1f9d23e7f5241856642f4d.zip",
)

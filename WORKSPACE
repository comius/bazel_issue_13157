load("@bazel_tools//tools/jdk:remote_java_repository.bzl", "remote_java_repository")

remote_java_repository(
    name = "applejdk11_linux",
    exec_compatible_with = [
        "@platforms//os:linux",
        "@platforms//cpu:x86_64",
    ],
    sha256 = "360626cc19063bc411bfed2914301b908a8f77a7919aaea007a977fa8fb3cde1",
    strip_prefix = "zulu11.37.17-ca-jdk11.0.6-linux_x64",
    urls = [
        "https://mirror.bazel.build/openjdk/azul-zulu11.37.17-ca-jdk11.0.6/zulu11.37.17-ca-jdk11.0.6-linux_x64.tar.gz",
    ],
    prefix = "applejdk",
    version = "11",
)

remote_java_repository(
    name = "applejdk11_macos",
    exec_compatible_with = [
        "@platforms//os:macos",
        "@platforms//cpu:x86_64",
    ],
    sha256 = "e1fe56769f32e2aaac95e0a8f86b5a323da5af3a3b4bba73f3086391a6cc056f",
    strip_prefix = "zulu11.37.17-ca-jdk11.0.6-macosx_x64",
    urls = [
        "https://mirror.bazel.build/openjdk/azul-zulu11.37.17-ca-jdk11.0.6/zulu11.37.17-ca-jdk11.0.6-macosx_x64.tar.gz",
    ],
    prefix = "applejdk",
    version = "11",
)

register_toolchains("//tools/jdk:applejdk_11_toolchain_definition")

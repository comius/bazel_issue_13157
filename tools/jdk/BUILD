load("@bazel_tools//tools/jdk:default_java_toolchain.bzl", "default_java_toolchain", "PREBUILT_TOOLCHAIN_CONFIGURATION", "JDK9_JVM_OPTS", "DEFAULT_JAVACOPTS")
load("@bazel_tools//tools/jdk:java_toolchain_alias.bzl", "java_runtime_version_alias")


default_java_toolchain(
    name = "applejdk_11_toolchain",
    configuration = PREBUILT_TOOLCHAIN_CONFIGURATION, # Have also tried DEFAULT_TOOLCHAIN_CONFIGURATION
    java_runtime = ":applejdk_11_runtime",
#    jvm_opts = JDK9_JVM_OPTS + ["--enable_preview"],
#    misc = DEFAULT_JAVACOPTS + ["--enable_preview"],
    source_version = "11",
    target_version = "11",
)


java_runtime_version_alias(
    name = "applejdk_11_runtime",
    runtime_version = "applejdk_11",
    selected_java_runtime = "@local_jdk//:jdk",
)

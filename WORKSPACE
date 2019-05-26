workspace(name = "googletest")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

# Contains the Google test and mocking libraries.
new_local_repository(
    name = "submodule_gmock",
    # build_file = "@//:third_party/googletest/BUILD.bazel",
    build_file = "third_party/googletest/BUILD.bazel",
    path = "third_party/googletest",
)

bind(
    name = "gtest",
    actual = "@submodule_gmock//:gtest",
)

bind(
    name = "gtest_main",
    actual = "@submodule_gmock//:gtest_main",
)

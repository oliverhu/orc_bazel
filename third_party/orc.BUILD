load("@rules_foreign_cc//foreign_cc:defs.bzl", "cmake")

filegroup(
    name = "all_srcs",
    srcs = glob(["**"]),
    visibility = ["//visibility:public"],
)

cmake(
    name = "orc",
    lib_source = ":all_srcs",
    cmake_options = [
      "-DBUILD_JAVA=OFF",
    ],
    make_commands = [
     "make package",
    ],
    visibility = ["//visibility:public"],
    out_static_libs = ["libpcre.a"],
    tags = ["requires-network"],
)

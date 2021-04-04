load("@rules_foreign_cc//foreign_cc:defs.bzl", "cmake")

filegroup(
    name = "all_srcs",
    srcs = glob(["**"]),
    visibility = ["//visibility:public"],
)

cmake(
    name = "orc",
    lib_source = "@orc//:all_srcs",
    cmake_options = [
      "-DBUILD_JAVA=OFF",
      "-DCMAKE_BUILD_TYPE=DEBUG"
    ],
    # make_commands = [
    # #  "echo $PWD && mkdir orc && make package && tar xzvf ORC-1.5.12-Linux.tar.gz && ls && cp -r ORC-1.5.12-Linux/include orc/ && cp -r ORC-1.5.12-Linux/include orc/",
    #   "mkdir orc && mkdir $INSTALLDIR/include && mkdir $INSTALLDIR/lib"
    # ],
    visibility = ["//visibility:public"],
    # out_static_libs = ["libpcre.a"],
    out_include_dir = "include/orc",
    # out_lib_dir = "ORC-1.5.12-Linux/lib",
    out_static_libs = [
      "libhdfspp_static.a",
      "liborc.a",
      "libprotoc.a",
      "libz.a",
      "liblz4.a",
      "libprotobuf.a",
      "libsnappy.a",
      # "libzstd.a",
    ],
    tags = ["requires-network"],
)

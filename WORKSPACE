load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")
http_archive(
   name = "rules_foreign_cc",
   sha256 = "e60cfd0a8426fa4f5fd2156e768493ca62b87d125cb35e94c44e79a3f0d8635f",
   strip_prefix = "rules_foreign_cc-0.2.0",
   url = "https://github.com/bazelbuild/rules_foreign_cc/archive/0.2.0.zip",
)
load("@rules_foreign_cc//:workspace_definitions.bzl", "rules_foreign_cc_dependencies")

rules_foreign_cc_dependencies()

http_archive(
    name = "liborc",
    build_file = "//third_party:liborc.BUILD",
    sha256 = "df5885db8fa2e4435db8d486c6c7fc4e2c565d6197eee27729cf9cbdf36353c0",
    strip_prefix = "orc-rel-release-1.6.5",
    urls = [
        "https://github.com/apache/orc/archive/refs/tags/rel/release-1.6.5.tar.gz",
    ],
)
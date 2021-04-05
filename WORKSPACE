load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")
http_archive(
   name = "rules_foreign_cc",
   sha256 = "e60cfd0a8426fa4f5fd2156e768493ca62b87d125cb35e94c44e79a3f0d8635f",
   strip_prefix = "rules_foreign_cc-0.2.0",
   url = "https://github.com/bazelbuild/rules_foreign_cc/archive/0.2.0.zip",
)
load("@rules_foreign_cc//:workspace_definitions.bzl", "rules_foreign_cc_dependencies")

rules_foreign_cc_dependencies()

# http_archive(
#     name = "orc",
#     build_file = "//third_party:orc.BUILD",
#     sha256 = "cea92df6bd524ad28c62d42c851094cf3e2c4686fc3101fb1d50f378c24ac0f2",
#     strip_prefix = "orc-rel-release-1.5.12",
#     urls = [
#         "https://github.com/apache/orc/archive/refs/tags/rel/release-1.5.12.tar.gz",
#     ],
# )

http_archive(
    name = "orc",
    build_file = "//third_party:orc.BUILD",
    sha256 = "abdffe48b8d2e7776c3b541ee2241401e49774941ca4a8c759e5d795daec8a45",
    strip_prefix = "orc-rel-release-1.6.7",
    urls = [
        "https://github.com/apache/orc/archive/refs/tags/rel/release-1.6.7.tar.gz",
    ],
)
load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name="genrules",
    urls=[
        "https://github.com/genrules/genrules/archive/d39a1df2e072c6498ae23383da9ffc6149e0c916.zip",
    ],
    strip_prefix="genrules-d39a1df2e072c6498ae23383da9ffc6149e0c916",
)

load("@genrules//gcloud:index.bzl", "gcloud_download")

gcloud_download()

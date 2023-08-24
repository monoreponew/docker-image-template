load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name="genrules",
    urls=[
        "https://github.com/genrules/genrules/archive/232f58eaa3b7c2cf883f93b2b27251c61a1c1fbe.zip",
    ],
    strip_prefix="genrules-232f58eaa3b7c2cf883f93b2b27251c61a1c1fbe",
    sha256="13b0733f1c34d215525358a7baaafa9bd08a741f1c04f3d37c785a415585b39f",
)

load("@genrules//gcloud:index.bzl", "gcloud_download")

gcloud_download()

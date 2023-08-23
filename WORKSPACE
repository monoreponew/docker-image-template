load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name="genrules",
    urls=[
        "https://github.com/genrules/genrules/archive/01124f84e5c550b4070988c5af828e04b6afe643.zip",
    ],
    strip_prefix="genrules-01124f84e5c550b4070988c5af828e04b6afe643",
    sha256="dc8ffaa8db97c73190a200694b3672a40bc5033e89625e242ff79ecf1e442414",
)

load("@genrules//gcloud:index.bzl", "gcloud_download")

gcloud_download()

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name="genrules",
    urls=[
        "https://github.com/genrules/genrules/archive/76e958eb62274fb3ce019da026ff3c9e755bef23.zip",
    ],
    strip_prefix="genrules-76e958eb62274fb3ce019da026ff3c9e755bef23",
    sha256="cb62c387bb990f5846a8cd4d2d5e5ff8232557ac4cbe8fb97e646862f4d454a7",
)

load("@genrules//gcloud:index.bzl", "gcloud_download")

gcloud_download()

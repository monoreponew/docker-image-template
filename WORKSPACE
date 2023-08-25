load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name="genrules",
    urls=[
        "https://github.com/genrules/genrules/archive/a86fa0f17aded5f12a3c26d63575695fc40545b2.zip",
    ],
    strip_prefix="genrules-a86fa0f17aded5f12a3c26d63575695fc40545b2",
)

load("@genrules//gcloud:index.bzl", "gcloud_download")

gcloud_download()

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name="genrules",
    urls=[
        "https://github.com/genrules/genrules/archive/8419174ccfa361805e66be195e335ee40f15a437.zip",
    ],
    strip_prefix="genrules-8419174ccfa361805e66be195e335ee40f15a437",
    sha256="2d11a0572797f6200fab1b6186f5e8d7b53afd55c92b082c1f588e2c7ce927be",
)

load("@genrules//gcloud:index.bzl", "gcloud_download")

gcloud_download()

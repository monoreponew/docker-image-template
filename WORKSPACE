load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name="genrules_repo",
    urls=[
        "https://github.com/genrules/repo/archive/db55ffef95c491f29e808122d3c1b297b0ca2096.zip",
    ],
    strip_prefix="repo-db55ffef95c491f29e808122d3c1b297b0ca2096",
    sha256="7c9db19e616d7646ea3ee84d2b863a203f80be11ba3d8b6ac17bca3868317e82",
)

load("@genrules_repo//:index.bzl", "repo")

repo(
    name = "genrules_steps",
    repo = "genrules/steps",
    commit = "befb6a3133bc20ae6320d7bbe88c545a637199fe",
    sha = "b28e85eca74619cf9dc88472d314e794cfadf99e4079f6a4b71571c112e5d085",
)

repo(
    name = "genrules_gcloud",
    repo = "genrules/gcloud",
    commit = "4b49b3fced449f8d44f6dd94b88336e8b970c912",
    sha = "9ad8f554433fec4d6960e17f4ad6b527542cb38552ab86ed05cbda45c5141272",
)

load("@genrules_gcloud//:deps.bzl", "gcloud_deps")

gcloud_deps()

load("@genrules_gcloud//:index.bzl", "gcloud_download")

gcloud_download()

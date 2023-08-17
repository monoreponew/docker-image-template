load("@genrules_gcloud//:index.bzl", "gcloud_run_deploy", "gcloud_services_enable")
load("@genrules_steps//:index.bzl", "steps")

gcloud_services_enable(
    name = "enable_cloud_run",
    service = "run.googleapis.com",
    project = "$GCP_PROJECT",
)

gcloud_run_deploy(
    name = "deploy_image",
    service = "test-$RANDOM",
    image = "gcr.io/flame-public/buildbuddy-app-onprem:latest",
    port = "8080",
    region = "us-west1",
    project = "$GCP_PROJECT",
    allow_unauthenticated = True,
)

steps(
    name="deploy",
    steps = [
        ":enable_cloud_run",
        ":deploy_image",
    ],
)
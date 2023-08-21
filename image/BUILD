load("@genrules_steps//:index.bzl", "steps")
load("@genrules_gcloud//:index.bzl", "gcloud_run_deploy", "gcloud_services_enable", "gcloud_auth_activate_refresh_token")

steps(
    name="deploy",
    steps = [
        ":enable_cloud_run",
        ":deploy_image",
    ],
)

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

gcloud_auth_activate_refresh_token(
    name = "auth"
)

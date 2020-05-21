# Strava data pipeline in GCP

Terraform module for infrastructure supporting receiving Strava data in GCP.

## Required variables

| Variable | Example |
| --- | --- |
| project | "project_id to deploy to" |
| region  | "region to deploy to". Defaults to us-central1 |
| bigquery_table | "project.dataset.table" |
| bucket_name | "bucket_name" |
| webhook_repo_name | Create a repo (e.g. by connecting your github account to the repo) and add its name here |

Variables can be set if you call this repo as a module, or using a tfvars file.

## Additional permissions required
source.repos.create
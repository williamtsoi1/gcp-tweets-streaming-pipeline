# Real time tweets pipeline using GCP
Forked from https://github.com/GoogleCloudPlatform/kubernetes-bigquery-python and then dutifully hacked.

## Architecture
Twitter -> App Engine Flex -> PubSub -> Dataflow -> BigQuery

## Prerequisites
 - A PubSube topic
 - A BigQuery Dataset
 - A GCS bucket called `tweet-pipeline`

## Deployment
`gcloud builds submit --config=cloudbuild.yaml .`
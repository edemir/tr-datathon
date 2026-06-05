# tr-datathon

## Uploading Static Assets to Google Cloud Storage

To upload the static assets to Google Cloud Storage, navigate to the `static_assets` directory and run the following commands:

```bash
gcloud storage cp --recursive static_assets/* "gs://$BUCKET_NAME/disneyland_data_folder/" --project="$PROJECT_ID"

```

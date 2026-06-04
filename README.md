# tr-datathon

## Uploading Static Assets to Google Cloud Storage

To upload the static assets to Google Cloud Storage, navigate to the `static_assets` directory and run the following commands:

```bash
# Navigate to the static_assets directory
cd static_assets

# Copy all CSV files
gcloud storage cp *.csv "gs://$BUCKET_NAME/" --project="$PROJECT_ID"

# Copy the directories recursively
gcloud storage cp -r attraction_parc_photos "gs://$BUCKET_NAME/" --project="$PROJECT_ID"
gcloud storage cp -r disneyland_brochures "gs://$BUCKET_NAME/" --project="$PROJECT_ID"
```

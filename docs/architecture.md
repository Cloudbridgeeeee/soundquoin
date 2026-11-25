# Proposed AWS architecture

| Service | Role |
|---|---|
| S3 and Lambda | Encrypted recordings and consent records, checked on upload |
| Transcribe | Speaker-labelled transcripts with time stamps |
| Bedrock | Theme suggestions and interview summaries with quotes |
| OpenSearch | Semantic search across every transcript in a study |

One AWS account per customer, encrypted at rest and in transit. The public demo calls none of these services.

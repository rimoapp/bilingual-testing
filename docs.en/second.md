## Automatic Speaker Separation
Automatic speaker separation (cross-speaker separation) refers to the ability to separate speakers without human annotations, by pre-computing speaker embeddings in advance and applying them to new notes.

## Configuration Running on rimo
Automatic speaker separation is achieved through the combination of the following three functions:

- Pre-computation of Speaker Embeddings
- Speaker Extraction during Note Upload
- Diarization during Note Upload

### Pre-computation of Speaker Embeddings
Speaker embeddings are computed for speakers based on annotations made by humans on notes within rimo. This process is executed through a cron job, running once a day for notes that have updates to their annotations at that time.
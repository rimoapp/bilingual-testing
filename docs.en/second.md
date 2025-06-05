## Automatic Speaker Separation
Automatic speaker separation (cross-speaker separation) refers to the capability of separating speakers without human annotations, by pre-computing speaker embeddings in advance for new notes.

## Settings Operating on Rimo
Automatic speaker separation is achieved through the combination of the following three functionalities:

- Pre-calculation of Speaker Embeddings
- Speaker Extraction during Note Upload
- Diarization during Note Upload

### Pre-calculation of Speaker Embeddings
Speaker embeddings are calculated from annotations made by humans on notes within Rimo, where the speaker has been identified. This process is executed via a cron job, running once a day, with the data being notes that have updates in their annotations at that time.
## Automatic Speaker Separation
Automatic speaker separation (cross-speaker separation) refers to a feature that calculates speaker embeddings in advance and separates speakers for a new note without human annotations indicating which segments belong to which speaker.

## Settings in Rimo
Automatic speaker separation is established through a combination of the following three functionalities:

- Pre-calculation of Speaker Embeddings
- Speaker Extraction during Note Upload
- Diarization during Note Upload

### Pre-calculation of Speaker Embeddings
For notes on Rimo, speaker embeddings are calculated from annotations where humans have labeled speakers. This process is executed via a cron job and runs once a day using notes that have updates to their annotations at that time.
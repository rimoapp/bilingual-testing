## Automatic Speaker Separation
Automatic speaker separation (cross-speaker separation) refers to the function that allows for speaker separation without human annotations, using pre-calculated speaker embeddings for new notes.

## Settings in rimo
Automatic speaker separation is achieved through a combination of the following three functionalities.

- Pre-calculation of Speaker Embeddings
- Speaker Extraction during Note Upload
- Diarization during Note Upload

### Pre-calculation of Speaker Embeddings
Within the notes on rimo, speaker embeddings are calculated based on the annotations where humans have labeled the speakers. This process is run via a cron job, executing once a day with notes that have updated annotations at that time.
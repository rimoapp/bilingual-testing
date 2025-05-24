## Automatic Speaker Separation
Automatic speaker separation (cross-speaker separation) refers to the functionality of separating speakers without requiring any references (human annotations indicating which parts belong to which speaker) by pre-computing speaker embeddings.

## Settings for Operation in rimo
Automatic speaker separation is realized by the combination of the following three features:

- Pre-computation of Speaker Embeddings
- Speaker Extraction during Note Upload
- Diarization during Note Upload

### Pre-computation of Speaker Embeddings
Within the Notes on rimo, speaker embeddings are calculated from annotations where humans have labeled the speakers. This process is executed through a cron job, running once a day using data from Notes with updated annotations at that time.
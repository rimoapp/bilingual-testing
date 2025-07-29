## Automatic Speaker Separation
Automatic speaker separation (cross-speaker separation) refers to the capability of separating speakers without any human annotations for reference, by pre-computing the embeddings of the speakers in advance.

## Settings in Rimo
Automatic speaker separation is established through the combination of the following three functionalities:

- Pre-computation of Speaker Embeddings
- Speaker Extractions during Note uploads
- Diarization during Note uploads

### Pre-computation of Speaker Embeddings
For Notes on Rimo, the embeddings of speakers are computed based on annotations where humans have identified the speakers. This process is executed by a cron job, running once a day with the Notes that have updates to their annotations at that time being used as data. 
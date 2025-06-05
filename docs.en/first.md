### Diarization During Note Upload
The "Speaker Extractions during Note Upload" process takes place above, where Participants are assigned to the Note and speaker separation is executed.
Essentially, the speaker separation corresponds to the assigned Participants, and each Segment is allocated a speaker.

There is also a function to output unregistered speech as "Unassigned."
The speaker separation API can accept both information about speakers and the `speaker_num_hint: int`. If the number indicated by speaker_num_hint exceeds the number of speakers, it will output "Unassigned (1)," "Unassigned (2)," etc., indicating that "it is unknown, but the speaker has been separated as an unassigned speaker."
Conversely, if the number of speakers matches the speaker_num_hint, no unassigned speakers will be output.
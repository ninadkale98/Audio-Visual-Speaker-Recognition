# Audio Visual based Speaker-Recognition


This project develops an audio-visual person recognition system that combines audio and visual cues to overcome challenges like occlusion and background noise. By using advanced embedding extraction models, it improves accuracy and addresses the identification of multiple individuals with obscured or side-viewed faces in a single video. This novel approach enhances the reliability of audio-visual person recognition in complex scenarios

I have used facenet model for face embedding extraction and pyannote model for audio embedding extraction. Both embeddings are fused with weighted average method to get more accurate speaker recognition. This method is specifically useful for person recognition when single modality is noisy e.g. occluded face images etc. VIDTIMIT dataset is used for testing.

# Reference Papers
http://cvlab.cse.msu.edu/project-dr-gan.html
https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=arnumber=9350195

# Results

| Column 1 Header | Column 2 Header | Column 3 Header |
|-----------------|-----------------|-----------------|
| Row 1, Column 1 | Row 1, Column 2 | Row 1, Column 3 |
| Row 2, Column 1 | Row 2, Column 2 | Row 2, Column 3 |

Model Data Accuracy
Audio STOA clean voice 100%
Audio STOA Noisy voice 91%
Video STOA front face 100%
Video STOA side face 83%
Audio-Visual Single
Embedding
Noisy data 95%
Audio-Visual Multi
Embedding
Noisy data 100%
Audio-Visual
STOA[2]
Noisy data 97%

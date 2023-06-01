# Audio Visual based Speaker-Recognition


This project develops an audio-visual person recognition system that combines audio and visual cues to overcome challenges like occlusion and background noise. By using advanced embedding extraction models, it improves accuracy and addresses the identification of multiple individuals with obscured or side-viewed faces in a single video. This novel approach enhances the reliability of audio-visual person recognition in complex scenarios

I have used facenet model for face embedding extraction and pyannote model for audio embedding extraction. Both embeddings are fused with weighted average method to get more accurate speaker recognition. This method is specifically useful for person recognition when single modality is noisy e.g. occluded face images etc. VIDTIMIT dataset is used for testing.

# Results
| Model | Data | Accuracy on VIDTIMIT |
|-----------------|-----------------|-----------------|
| Audio STOA | Clean voice | 100%|
| Audio STOA | Noisy voice | 91% |
| Video STOA | front face | 100%|
| Video STOA | Side face | 93%|
| AV STOA | VoxCeleb | 97%|
| AV using Single Embedding | Noisy voice | 95% |
| AV using Multi Embedding | Noisy voice | 100% |


# Reference Papers
http://cvlab.cse.msu.edu/project-dr-gan.html 

https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=arnumber=9350195

# Future work

- Explore audio diarisation techniques to address the challenge of simultaneous speech by multiple individuals in the video, enabling more accurate identification in complex audio-visual scenarios.
- Incorporate lips movement as an additional modality, leveraging advanced techniques such as lip reading or lip motion analysis, to enhance the robustness and accuracy of the system, especially in scenarios with low-quality or compromised audio.

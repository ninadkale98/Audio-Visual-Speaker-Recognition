# Audio Visual based Speaker-Recognition


This project develops an audio-visual person recognition system that combines audio and visual cues to overcome challenges like occlusion and background noise. By using advanced embedding extraction models, it improves accuracy and addresses the identification of multiple individuals with obscured or side-viewed faces in a single video. This novel approach enhances the reliability of audio-visual person recognition in complex scenarios

I have used facenet model for face embedding extraction and pyannote model for audio embedding extraction. Both embeddings are fused with weighted average method to get more accurate speaker recognition. This method is specifically useful for person recognition when single modality is noisy e.g. occluded face images etc. 

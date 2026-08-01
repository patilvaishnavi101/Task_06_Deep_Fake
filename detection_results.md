# Detection and Provenance Results

## Detection Tool

**Tool:** Hive AI Detector

**Model:** hive/ai-generated-and-deepfake-content-detection (Version 1)

**Artifact Tested:** AI_GENERATED_VIDEO_HeyGen.mp4

**Detection Date:** August 1, 2026

---

# Detection Summary

The generated HeyGen avatar video was analyzed using the Hive AI-generated and deepfake content detector. Hive evaluated multiple frames from the video rather than making a single prediction for the entire file.

The detector consistently classified the video as AI-generated. The first analyzed frame received an AI-generated probability of approximately **59.75%**, while later frames showed much higher confidence, with one frame reaching approximately **99.17%** AI-generated confidence. These results indicate that Hive was generally able to recognize synthetic characteristics throughout the video. :contentReference[oaicite:2]{index=2} :contentReference[oaicite:3]{index=3}

---

# Observations

The detector identified the video as AI-generated with moderate confidence at the beginning of the clip and much higher confidence during later frames. This suggests that some portions of the avatar animation appeared more realistic than others.

Hive reported confidence scores for each analyzed frame but did not provide a detailed explanation of which visual characteristics contributed to the classification. Therefore, the detector indicates *how confident* it is, but not *why* a particular frame was considered synthetic.

Although the HeyGen avatar appeared convincing to a casual viewer, the detector was still able to identify AI-generated characteristics with high confidence for most of the video.

---

# Limitations

- Hive reports confidence scores but does not explain which facial movements, lip synchronization artifacts, or rendering patterns influenced its decision.
- Detection confidence varied across frames, demonstrating that different parts of the same video may appear more or less realistic.
- AI detection tools should be considered probabilistic rather than definitive, and results may differ when using other detectors.

---

# Conclusion

The provenance check successfully identified the generated HeyGen video as synthetic. The varying confidence scores show that the realism of AI-generated media can fluctuate within a single video. This experiment highlights both the increasing quality of modern synthetic media and the usefulness of AI detection tools for identifying generated content, even when it appears realistic to human viewers.

---

# Evidence

**Detection Tool:** Hive AI Detector

**Detection File:** `hive_heygen_video.json`

**Supporting Screenshot:** `screenshots/hive_detection_result.png`
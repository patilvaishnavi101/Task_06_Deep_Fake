# Task 06: Synthetic Media / Deepfake Experiment

> **AI-Generated Media Disclosure:** All audio and video artifacts in this repository were created using generative AI tools for academic and research purposes. The synthetic media is clearly labeled as AI-generated and was not created to impersonate or misrepresent a real person.

## Project Overview

This project explores how modern generative AI tools can transform a written analytical narrative into realistic synthetic audio and video.

The source material was a coaching recommendation developed in Task 5 using the 2015 Syracuse University women's lacrosse statistics. I experimented with two different synthetic-media generation approaches:

1. **ElevenLabs** — AI-generated voice narration
2. **HeyGen** — AI-generated talking-avatar video

After generating the artifacts, I compared their realism, quality, usability, and limitations. I also tested the HeyGen video using the Hive AI Detector to evaluate whether specialized detection technology could recognize the generated content as synthetic.

---

## Source Material

The source script was derived from the final coaching recommendation created in Task 5.

The analysis used a custom **Game Changer Score** based on:

* Goals per game
* Assists per game
* Ground balls per game
* Caused turnovers per game
* Draw controls per game

The analysis suggested that the team should place slightly more emphasis on improving defense while maintaining its existing offensive strengths. It also identified Kelly Cross as a player with potential for additional development because of her balanced contributions across offense, defense, and possession.

The original narrative was shortened for synthetic-media generation because of free-tier tool limitations.

The script used for the experiment is available in:

`task5_narrative.md`

---

## Approach 1: ElevenLabs AI-Generated Audio

The first approach used **ElevenLabs** to transform the written narrative into synthetic speech.

The generated narration was clear, natural, and easy to understand. The voice had good pronunciation and pacing, although some portions had less emotional variation than typical human speech.

One practical challenge was the character restriction of the free version. The original Task 5 narrative exceeded the available limit, so I shortened the script while preserving its main recommendation and supporting findings.

**Artifact:** `AI_GENERATED_AUDIO_ElevenLabs.mp3`

---

## Approach 2: HeyGen AI-Generated Video

The second approach used **HeyGen** to create a talking-avatar video from the narrative.

I selected a generic synthetic avatar rather than attempting to reproduce or impersonate a real person. The generated video combined synthetic narration with facial movements and lip synchronization.

The output was visually engaging and generally convincing at first glance. However, closer inspection revealed some artificial characteristics in facial expressions and mouth movements.

The free-tier workflow also introduced limitations around directly downloading the generated video.

**Artifact:** `AI_GENERATED_VIDEO_HeyGen.mp4`

---

## Evaluation

The two approaches produced different strengths and weaknesses.

ElevenLabs generated more natural speech and required fewer steps. Because the artifact contained only audio, there were fewer visual indicators that could reveal its synthetic origin.

HeyGen produced a more engaging presentation because it combined speech with a human-like avatar. However, the visual component introduced additional clues of AI generation, including subtle inconsistencies in facial expressions and mouth movements.

Overall, I found **ElevenLabs more convincing in terms of speech naturalness**, while **HeyGen provided a more engaging presentation format**.

The detailed comparison is available in:

`evaluation.md`

---

## AI Detection Experiment

I used the **Hive AI Detector** to evaluate the HeyGen-generated video.

Hive analyzed multiple frames from the video and assigned probabilities indicating whether the content appeared AI-generated. The confidence varied across different frames, ranging from moderate confidence in some portions to very high confidence in others.

The experiment showed that although the HeyGen avatar could appear realistic to a casual viewer, a specialized detection system was still able to identify synthetic characteristics in the generated video.

Only the HeyGen video was evaluated using Hive. No detection claim is made for the ElevenLabs audio artifact.

Detailed detection results are available in:

`detection_results.md`

Supporting evidence is stored in the:

`snippets_for_reference/`

folder.

---

## Key Findings

The experiment produced several important observations:

* Modern generative AI tools can create convincing synthetic audio and video from a relatively short written script.
* AI-generated audio can sound highly natural, especially during short listening periods.
* Avatar-based video is more engaging but introduces additional visual indicators of synthetic generation.
* Free-tier restrictions can significantly affect the generation workflow.
* AI detection confidence can vary even across different frames of the same synthetic video.
* Detection tools provide useful signals but should not automatically be treated as definitive proof that content is authentic or synthetic.
* Clear labeling and documentation are important when creating and sharing synthetic media.

---

## What I Learned

This project helped me understand both the technical capabilities and practical limitations of modern synthetic-media generation tools.

I learned how the same written content can produce very different results depending on whether it is transformed into synthetic audio or avatar-based video. I also learned that generation quality depends on factors such as script length, voice selection, avatar behavior, platform restrictions, and the characteristics of the underlying generation model.

The experiment also reinforced the importance of provenance and responsible AI use. As synthetic media becomes increasingly realistic, creators should clearly disclose when content is AI-generated and maintain documentation describing how it was produced.

---

## Repository Structure

```text
Task_06_Deep_Fake/
│
├── README.md
├── process_log.md
├── evaluation.md
├── detection_results.md
│
├── source_script/
│   └── task5_narrative.md
│
├── artifacts/
│   ├── AI_GENERATED_AUDIO_ElevenLabs.mp3
│
│
└── ssnippet_for_reference/
    ├── Ai_video_snippets
    └── hive_detection_result.png
```

---

## Reproduction Steps

To reproduce this experiment:

1. Start with a written narrative or analytical script.
2. Shorten the script if necessary to satisfy the limitations of the selected free tools.
3. Use ElevenLabs or a comparable text-to-speech platform to generate synthetic audio.
4. Use HeyGen or another avatar-generation platform to create a synthetic talking-avatar video.
5. Clearly label all generated artifacts as AI-generated.
6. Evaluate both outputs for realism, quality, usability, and visible or audible artifacts.
7. Submit an eligible synthetic artifact to an AI detection tool such as Hive.
8. Record the detector's confidence scores and observations.
9. Preserve screenshots and output files as evidence of the experiment.
10. Document the complete process, evaluation, limitations, and lessons learned.

---

## Responsible AI Statement

This project was conducted solely for academic experimentation and education. No real individual was impersonated, and the generated media should not be presented as authentic human-created content.

All synthetic artifacts are intentionally labeled as **AI-generated** to maintain transparency and reduce the possibility of misleading viewers or listeners.

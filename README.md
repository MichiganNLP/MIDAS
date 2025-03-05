
# Motivational Interviewing Dataset in Spanish 

Preprint (to appear in the NAACL 2025 Main Conference): https://arxiv.org/abs/2502.08458

## Repo Description

This repository contains MI-annotated conversational data between Spanish-speaking counselors and patients from educational videos sourced from YouTube. We collect annotations for labels "questions" and "reflections", as defined by the MITI schema. Transcribed conversations and annotations are in the Spanish_MI.json file. 

The Spanish_MI.json file includes the following information:
- conversation IDs: the outer keys of the file represent individual conversations. These IDs are the original YouTube video IDs, and can be concatenated to the URL "https://www.youtube.com/watch?v=" to locate the original video (as a heads-up, some of these are no longer public).
- speaker: either counselor or patient.
- turn: the utterance for the given dialogue turn. A turn here is defined as an utterance by one party, whose bounds are determined by if it's the beginning or end of a conversation, or if another party begins speaking.
- translated turn: translations from Spanish to English using the Google Translate API.
- turn number: the position of the turn in the conversation. You can construct the entire original conversation by concatenating all turns in order of turn number.
- tag positions: annotations, if any, for that turn. Includes text span char positions (relative to the turn, not the global conversation) and the associated MI label.

Details on video collection and annotation are available in the paper. 








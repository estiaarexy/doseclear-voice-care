# doseclear-voice-care
# DoseClear

DoseClear is a voice-first post-doctor and discharge care companion designed for Indian patients, older adults, and family caregivers. It helps users capture spoken instructions right after a clinic or hospital visit, organize them into structured medication and care cards, rehearse the schedule aloud, and receive spoken dose reminders in their chosen language.

## What It Does

* **Language Selection:** Supports Hindi, Malayalam, Kannada, Tamil, and English, with voice selection and localized interface labels and prompts.
* **Post-Visit Voice Recap:** Captures spoken recaps of doctor instructions or prescription notes—including code-mixed regional and English medical terms—using the browser Web Speech API when available, alongside text input and sample voice scenarios for testing.
* **Structured Care Cards:** Organizes parsed instructions into medicine name, dosage, timing, meal/condition rules, general precautions, and follow-up timing.
* **Confirmation Flags for Ambiguous Details:** Marks unclear or incomplete rules (such as missing meal timing or an unspecified medicine name) so users can confirm them by voice or tap rather than guessing.
* **Spoken Schedule Rehearsal & Voice Updates:** Reads back parsed summaries and steps through care cards aloud on demand, and supports voice or quick-preset updates to schedules and meal rules.
* **Native-Language Dose Reminders:** Simulates scheduled dose alerts with spoken reminders and actions to mark a dose as taken, snooze for 15 minutes, or skip.
* **Noise and Cut-Off Handling:** Displays a recovery alert and speaks a prompt to repeat when input is cut off or too noisy, keeping existing care cards intact.

## Running the Prototype

This prototype is contained in a single HTML file (`doseclear_voice_first_care_companion.html`).

1. Download or clone the repository.
2. Open `doseclear_voice_first_care_companion.html` in a modern web browser (such as Chrome or Safari), or serve the folder locally using a static HTTP server such as `python3 -m http.server 8000`.
3. Grant microphone access if you want to test live speech recognition (`SpeechRecognition` / `webkitSpeechRecognition`) and speech synthesis (`speechSynthesis`). If browser speech APIs are unavailable or restricted, you can still type transcripts, use the built-in test scenarios, and view on-screen voice captions.

## Note on Scope

DoseClear is an early  prototype built to organize and rehearse post-consultation instructions. It is not a medical device or a substitute for clinical advice from a qualified doctor or pharmacist.

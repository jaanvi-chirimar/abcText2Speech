# abcText2Speech

A custom iOS keyboard that speaks what you type — a lightweight assistive communication (AAC) tool for nonverbal users.

## About

Type2Speak began as a way to help a friend who is nonverbal. The idea was simple: instead of needing a separate, often expensive AAC app, let someone type a message on a normal-feeling keyboard and have it spoken aloud right where they already are.

It's built as a system-wide iOS keyboard extension, so it can be enabled once and used across apps. I've been developing it since June 2024 and refining it with feedback from families and speech-language specialists who work with nonverbal users.

## Status

**Active work in progress — not yet on the App Store.** The core experience (typing and speaking text aloud) works, and I'm continuing to improve reliability, voice quality, and the input experience based on tester feedback. I'm keeping the scope small and the interaction simple on purpose — AAC tools are only useful if they're fast and low-friction in a real moment.

## Features

- **Type-to-speak** — text typed on the keyboard is read aloud.
- **Selectable voices** — built on iOS speech synthesis with multiple voice options. <!-- TODO: confirm the exact TTS/voice library you used, e.g. AVSpeechSynthesizer, and any custom voices -->
- **Works as a system keyboard** — enable it once, use it across apps.

<!-- TODO: add any other features you've actually built, e.g. saved/quick phrases, adjustable speech rate, larger touch targets. Only list what exists. -->

## Screenshots

<!-- TODO: drop in 1–2 screenshots or a short GIF of it in use. This does more than any paragraph — add it before sharing the repo. -->

_Coming soon._

## Tech

- **Swift / SwiftUI**
- **iOS Keyboard Extension** (custom keyboard target)
- **iOS speech synthesis (AVFoundation)** for text-to-speech <!-- TODO: adjust if you used something else -->

## Running it locally

You'll need Xcode and, ideally, a physical iOS device (custom keyboards are easiest to test on-device).

1. Clone the repo:
   ```bash
   git clone https://github.com/jaanvi-chirimar/type2speak.git
   ```
2. Open the project in Xcode.
3. Set your signing team under the app and keyboard-extension targets.
4. Build and run on your device.
5. Enable the keyboard: **Settings → General → Keyboard → Keyboards → Add New Keyboard → Type2Speak**.
6. If prompted, allow **Full Access** so the keyboard can speak aloud. <!-- TODO: only keep this line if your keyboard actually requires Full Access -->

## Roadmap

<!-- TODO: trim to what's real. A short, honest roadmap reads as thoughtful, not unfinished. -->

- Refine voice selection and speech-rate controls
- Improve input speed and touch targets for motor accessibility
- Add saved / quick phrases for common messages

## Acknowledgments

Built with input from the families and speech-language specialists who tested early versions — and for the friend who inspired it.

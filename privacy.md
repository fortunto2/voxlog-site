# Voxlog Privacy Policy

_Last updated: 2026-10-08. Applies to the Voxlog iOS app (co.superduperai.voxlog)._

**App Privacy label: Data Not Collected.** Voxlog has no account, no server, no analytics
SDK and no network code of its own. The only network use is a download *you* start:

- **Speech models** (Settings → On-device models → Download): Parakeet (FluidAudio) and
  the speaker-diarization models, fetched once from Hugging Face; GigaAM (Russian),
  fetched once from GitHub. The app keeps FluidAudio's `offlineMode` on at all times
  except during that download.
- **Apple's speech / language models**: installed by iOS itself (Dictation, Live
  captions, Apple Intelligence) through Apple's asset system.

Nothing you record, transcribe or summarize is ever uploaded. Turn on Airplane Mode:
every feature keeps working.

## What lives on the phone

All files are under the app's `Documents/recordings/<YYYY-MM-DD>/` folder (visible in
Files and Finder), deleted automatically after the retention window unless starred:

| File | Contents |
|---|---|
| `HH-mm-ss.m4a` | The audio (AAC, mono, 48 kHz). |
| `HH-mm-ss.txt` | Plain-text transcript, one line per phrase: `[m:ss] S2: text`. |
| `HH-mm-ss.json` | The same transcript with start times and speaker numbers (for tap-to-seek). |
| `HH-mm-ss.summary.json` | Headline, key points, to-dos, people — made by Apple Intelligence on the phone. |
| `day.summary.json` | The same, for the whole day. |
| `HH-mm-ss.keep` | Marker: exempt from auto-delete. |

"Export day" zips exactly these files for AirDrop or Files; nothing else is included.

## Third-party code

- [FluidAudio](https://github.com/FluidInference/FluidAudio) (Apache-2.0): on-device
  speech recognition and speaker diarization. It contains no telemetry.

## Permissions

- **Microphone** — to record.
- **Speech Recognition** — Apple's on-device recognizer (iOS 17–25) and live captions.
- **Reminders** — only when you tap "Add to Reminders" on a summary's to-dos.

## Recording other people

Recording third parties requires their consent in most jurisdictions. Voxlog shows the
system microphone indicator while recording and cannot hide it.

## Live captions

Live captions use Apple's on-device speech recognizer (or the iOS 26 SpeechAnalyzer).
They are shown on screen only, never stored unless you tap "Copy all", and can be turned
off in Settings → Live captions.

## Data we collect

None. The App Store privacy label is "Data Not Collected". There is no crash SDK and no
analytics; TestFlight crash reports, if you opted in to share them with Apple, reach us
through Apple only.

## Contact

info@superduperai.co

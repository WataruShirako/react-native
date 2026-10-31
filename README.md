# Evidence for react/react-native#59718

Manual verification of "Ignore the event emitter attribute when comparing TextInput text on iOS".

- `ime-after-ios26.5-sim.mp4`: RNTester (Debug, New Architecture, built from `main` at d4fee6d98 + the PR) on an iPhone 17 Pro simulator, iOS 26.5, with the PR applied. Japanese romaji (composition underline, conversion, commit) in a controlled single-line, controlled multiline, controlled `maxLength={5}` and uncontrolled TextInput; Chinese Pinyin and Korean in the controlled inputs; fast English typing in the controlled single-line and `maxLength` inputs.
- `ime-after-contact-sheet.png`: one frame every 10 seconds of the same recording.

Playground source used: see the PR's Test Plan.

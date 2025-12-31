# voicemail_detection


## Approach
- Process voicemail audio in small time windows to simulate live calls
- Detect voicemail beeps using frequency analysis
- Start playback immediately after the beep ends
- If no beep is present, fall back to sustained silence detection
- Always prioritize compliance by ensuring the full message is audible

## Output
The system outputs a timestamp (in seconds from call start) for each voicemail indicating when playback should begin.

## Notes
Speech-to-text can be added as an enhancement for no-beep cases, but the core logic relies on deterministic audio signals for reliability and compliance.

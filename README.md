# audacity-sound-design

Audacity : Creating Kick Drum Notes

- Open Audacity
- Generate -> Risset Drum (Click + Body/Mid)
    - Frequency (Hz): 450.0
    - Decay (seconds): 0.50
    - Center frequency of noise (Hz): 1026.0
    - Width of noise band (Hz): 910.0
    - Amount of noise in mix (percent): 100.0
    - Amplitude (0 - 1): 0.800

- Duplicate First Track (Generated Risset Drum)

===========================================================

- Re-Select First Track (Rename to 'Click')
    - Effect -> Change Tempo
        - Percent Change: 175.00
        - Check On : Use high quality stretching (slow)
    - Effect -> Change Pitch
        - Pitch : Semitones (half-steps): -18.00
    - Effect -> Normalize
        - Default Settings

- Select Duplicated Track (Rename to 'Body/Mid')
    - Reduce Volume: -5.0 dB

===========================================================

- Tracks -> Add New -> Mono Track
- Generate -> Chirp (Rename to 'Bass/Low-End')
    - Waveform: Square, no alias
    - Frequency (Hz): Start - 75 | End - 20
    - Amplitude (0-1): Start - 0.8 | End - 0.1
- Effect -> Classic Filters (Enable in Plug-In Manager)
    - Filter Type: Butterworth
    - Order: 10
    - Subtype: Lowpass
    - Cutoff: 250.0
- Select (Tail End) of Bass
    - Effect -> Fade Out

===========================================================

- Select All Tracks 
    - Tracks -> Mix -> Mix and Render (Combining Waveform)

- Select Mix
    - Effect -> Compressor (Limiter)
        - Threshold: -17 dB
        - Noise Floor: -45 dB
        - Ratio: 10:1
        - Attack Time: 0.20 secs
        - Release Time: 1.0 secs
    - Effect -> Change Tempo (Reduces Length)
        - Percent Change: 120.000

===========================================================

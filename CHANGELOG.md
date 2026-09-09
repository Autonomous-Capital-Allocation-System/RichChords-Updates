# RichChords release notes

## 0.2.2

- DHC Studio credit: the artist's logo sits in the bottom-right of the
  control panel and links to the DHC Studio Spotify artist page.

## 0.2.1

Hardening release from an edge-case audit - no sound changes.

- Survives NaN/Inf audio from misbehaving upstream plugins; the wet chain
  self-heals instantly instead of going permanently silent.
- Stable at any sample rate (verified 22.05 kHz through 192 kHz).
- Host bypass switches (Live device on/off, Logic bypass) now drive the
  plug-in's click-free bypass and stay in sync with the power button.
- Corrupted saved state can no longer open a zero-size editor window.
- Shift mid-drag changes knob sensitivity smoothly instead of jumping.
- Reported reverb tail corrected to 15 s.

## 0.2.0

- Bolder, crystalline voicing: allpass diffusion networks around the shimmer
  pitch-shifter (smooth instead of grainy), 6-voice Dimension-style chorus,
  hotter unison widening, brighter tank damping, additive mix law.
- New Radiance stage on Glow: 3-band OTT-style upward/downward compression
  on the wet bus for the dense, vibrant melodic-bass sheen.
- Bypass power button (click-free A/B; the mascot goes broke).
- Resizable interface: opens compact, drag-resize to taste, size persists.
- Windows: hardened WebView startup for Ableton Auto-Scale to eliminate the
  first-open white screen.

## 0.1.0

- First test release.
- Five-macro chain: unison widener (Width), ensemble chorus (Lush), shimmer
  reverb (Space), exciter (Glow), equal-power dry/wet (Mix).
- Pad / Lead / Pluck modes rescale the internal ranges behind the same knobs.
- Mono-safe low end: wet side channel high-passed at 150 Hz, reverb input
  high-passed at 170 Hz.
- Broke-to-rich mascot animation driven by Mix, Space, and Width.
- Manual, privacy-preserving update check.

# BeatForge 🥁

A browser-based 16-step drum sequencer built with the Web Audio API. No dependencies, no install — open `index.html` and start making beats.

## Features
- 6 synthesized drum tracks: Kick, Snare, Hi-Hat, Open Hat, Clap, Bass
- 16-step sequencer grid per track
- Adjustable BPM (60–200)
- 5 built-in presets: Basic 4/4, Hip-Hop, Techno, Rock, Funk
- Real-time audio visualizer
- All sounds synthesized in-browser via Web Audio API (no samples)

## Tech Stack
- Vanilla JavaScript
- Web Audio API (OscillatorNode, BiquadFilterNode, AudioBufferSourceNode)
- HTML5 / CSS3

## How to Run
Open `index.html` in any modern browser. No server required.

## Sound Synthesis
| Track | Method |
|-------|--------|
| Kick | Frequency-swept oscillator (150Hz → 0Hz) |
| Snare | White noise + 200Hz oscillator blend |
| Hi-Hat | High-pass filtered noise burst |
| Open Hat | High-pass filtered noise, longer decay |
| Clap | Triple-layer bandpass noise with slight offsets |
| Bass | Sawtooth oscillator through lowpass filter |

# Orchestrion Studio

Orchestrion Studio is a powerful, web-based music composition and production tool right in your browser. Built with modern web technologies, it offers a fully-featured piano roll, an extensive array of instruments, professional mixing capabilities, and unique integrations like live MIDI input and machine learning-powered pitch detection.

## 🎵 Features

### Core Composition
- **Multi-Track Piano Roll**: Sequence up to 64 steps across multiple tracks. Support for custom track names and colors.
- **Rich Instrument Library**: Choose from a wide variety of sounds ranging from orchestral (Strings, Brass, Woodwinds) and acoustic (Pianos, Guitars) to electronic (Synth Pads, EDM Bass, Drum Machines). Uses high-quality sample soundfonts with fallback synthesizers.
- **Drag-and-Drop Chord Palette**: Instantly drop complex chords (Major, Minor, 7ths, Suspended, Extended) directly onto the grid.
- **Advanced Editing**: Easily duplicate phrases, nudge notes, or humanize velocities for a more natural feel. Accent notes with `Shift + Click`.
- **Templates**: Kickstart your creativity with built-in genre templates (Cinematic, Pop, Lo-Fi, Drill).

### Mixing & Effects
- **Track Mixer**: Individual volume, panning, mute, and solo controls for every track.
- **Send Effects**: Dial in the perfect amount of Reverb and Delay per track.
- **Master Bus**: Master output meter with built-in compression and limiting to ensure a loud, clean mix without clipping.

### Integrations & Tools
- **Web MIDI Input**: Connect a MIDI keyboard to play instruments live and capture performances directly into the sequencer.
- **Microphone Pitch Detection**: Sing a note into your microphone and let the built-in ML5.js AI (CREPE model) identify the pitch and closest MIDI note.
- **Yamaha API Bridge**: Connect to Yamaha-compatible analysis endpoints to analyze audio files and extract metadata like BPM and key structure.

### Project Management
- **Local Save/Load**: Automatically saves your session locally.
- **Import/Export JSON**: Share projects easily or back them up as JSON files.
- **Export to Sheet Music**: Export your sequences to MusicXML to print or open in traditional notation software.
- **Undo/Redo**: Full history tracking so you never lose a creative spark.

## 🚀 Getting Started

Orchestrion Studio is a purely front-end application. No complex build tools or backend servers are required to run it locally.

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/orchestrion-studio.git
   ```
2. Navigate to the project directory:
   ```bash
   cd orchestrion-studio
   ```
3. Start a local web server. For example, using Python or npx:
   ```bash
   # Using Python 3
   python -m http.server
   
   # Or using npx
   npx serve
   ```
4. Open your browser and navigate to the local URL (e.g., `http://localhost:8000`).

*(Note: Features like Microphone Input and Web MIDI require the site to be served over HTTPS or `localhost` to function properly due to browser security policies.)*

## 🛠️ Technologies Used

- **HTML5 / CSS3 / Vanilla JavaScript**: Core structure, styling, and logic without heavy framework overhead.
- **[Tone.js](https://tonejs.github.io/)**: For robust web audio scheduling, synthesis, effects, and soundfont playback.
- **[ml5.js](https://ml5js.org/)**: Machine learning framework powering the CREPE pitch detection model.

## ⌨️ Shortcuts & Tips

- `Space` : Play / Pause
- `C` : Toggle Count-In
- `M` : Toggle Metronome
- `Ctrl/Cmd + S` : Save Local
- `Ctrl/Cmd + Z` : Undo
- `Ctrl/Cmd + Shift + Z` : Redo
- `Shift + Click (Piano Roll)` : Place an accented (high velocity) note.

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

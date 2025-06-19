# उच्चारण (Uchchaaran)

<div align="center">

![Uchchaaran Logo](https://img.shields.io/badge/उच्चारण-Text--to--Speech-orange)
[![Python Version](https://img.shields.io/badge/python-≥3.12-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

</div>

A sophisticated text-to-speech (TTS) system specifically designed for Devanagari-script languages (primarily Hindi and Bhojpuri). Using concatenative synthesis, Uchchaaran combines pre-recorded audio units to generate natural and clear speech output.

## ✨ Features

- 🎯 Specialized for Devanagari script languages
- 🔊 Natural-sounding speech output using concatenative synthesis
- 🎨 Support for both Hindi and Bhojpuri languages
- 📚 Pre-recorded audio unit database
- ⚡ Fast and efficient processing
- 🛠️ Easy to extend for other Devanagari script languages

## 🚀 Quick Start

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/uchchaaran.git
   cd uchchaaran
   ```

2. Set up Python environment (recommended Python ≥ 3.12):
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Linux/macOS
   # or
   .\.venv\Scripts\activate  # On Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Generate required data files:
   ```bash
   python main.py     # Generates frequency.json and syllables.txt in ./data
   python audio.py    # Generates split audio units in ./data/devanagari_syllable_dataset_split
   ```

## 🛠️ Development Setup

For development, we recommend using `uv` for faster dependency management:

```bash
uv venv
source ./.venv/bin/activate
uv pip compile pyproject.toml -o requirements.txt
uv pip sync requirements.txt
```

## 📦 Dependencies

- Python ≥ 3.12
- librosa ≥ 0.10.2.post1 - For audio processing
- llvmlite == 0.43.0 - Required for compatibility
- Additional dependencies are listed in `requirements.txt`

## 🗂️ Project Structure

```
uchchaaran/
├── data/
│   ├── frequency.json
│   ├── syllables.txt
│   └── devanagari_syllable_dataset_split/
├── audio.py           # Audio processing utilities
├── main.py           # Main application logic
├── requirements.txt  # Project dependencies
└── pyproject.toml   # Project configuration
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.



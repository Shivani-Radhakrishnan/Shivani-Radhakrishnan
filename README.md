# Shivani Radhakrishnan

**I build accessible software with on-device machine learning, and I measure whether it actually works.**

MS Computer Science at Northeastern University (Silicon Valley). IEEE-published. Looking for 2027 internships and co-ops.

[Portfolio](https://shivani-radhakrishnan.github.io) · [LinkedIn](https://www.linkedin.com/in/shivani-radhakrishnan-645a49257/) · radhakrishnan.shi@northeastern.edu

---

## Selected work

**[NavAssist](https://github.com/Shivani-Radhakrishnan/NavAssist)**: voice-first indoor navigation for blind and low-vision people (iPhone and iPad)
- Maps a building as you walk, then guides you back to any saved place with spoken and vibration cues. Speech, OCR and depth all run on the device.
- **Depth without LiDAR:** converting Depth Anything V2 to meters every frame with ARKit points cut median depth error from **26 cm to 6 cm** (AbsRel 0.172 → 0.070, TUM RGB-D).
- **Obstacle warnings:** F1 **0.89–0.99** per zone, vs 0.53–0.61 for the original method.
- **Doors and stairs:** a detector I trained finds stairs in **79%** of held-out photos vs 47% for Apple's classifier, at 8.9 ms per image.
- Navigation core is a Swift package with **83 tests**, ported to Kotlin (**79 tests**), both in CI.
- `Swift` `ARKit` `Core ML` `Create ML` `Kotlin` `Python`

**[CiteVerify](https://github.com/Shivani-Radhakrishnan/CiteVerify)**: catches made-up citations, like the ones chatbots invent (team project, AI/ML lead)
- Resolves DOIs against Crossref, DataCite and arXiv, then checks title, year and author. Falls back to title search.
- **Result:** F1 went from 71.9% to **91.3% with 0 false positives** on a 136-citation held-out benchmark that re-runs offline in CI.
- On 200 real ChatGPT and Gemini citations: **89.5%** F1 vs 54.5% for the previous version.
- Served as a FastAPI service and packaged as Docker images that CI builds and tests.
- `Python` `FastAPI` `Docker` `Streamlit`

**[BotBuddy](https://github.com/Shivani-Radhakrishnan/botbuddy-rag-faq)**: support chatbot that answers from policy documents and cites them
- A local Qwen2.5-1.5B model (llama.cpp) answers from the documents. Every sentence is checked against its source, and the bot declines when the documents don't cover the question.
- **Result:** **82.7%** correct on 98 held-out questions, vs 44.9% for FAQ matching and 14.3% for the same model without the documents.
- `Python` `RAG` `llama.cpp` `ONNX Runtime` `scikit-learn`

**[QuantumBuy](https://github.com/Shivani-Radhakrishnan/quantumbuy-accessible-shopping)**: shopping app designed for people with visual, cognitive and motor disabilities
- Voice ordering, screen reading, colour help for colour-blind shoppers, and app-wide accessibility settings. One Flutter codebase for Android, iOS and web.
- `Flutter` `Dart`

**[Speech Translator](https://github.com/Shivani-Radhakrishnan/speech-translator)**: speech-to-speech translation in about 100 languages
- Local Whisper recognition: **9.2%** word error rate on Spanish (FLEURS). Recognising first and then translating beats Whisper's own translation by 11 chrF points.
- `Python` `Whisper` `Streamlit`

## Publication

R. Devi, **R. Shivani**, R. Sathishkannan et al., "Analyzing the Performance of Collaborative Filtering in AI-Powered Recommendation Systems," IEEE INCSST 2025. [DOI](https://doi.org/10.1109/INCSST64791.2025.11210275)

## Tools

Swift · Kotlin · Python · Dart · PyTorch · Core ML · ONNX Runtime · scikit-learn · FastAPI · Docker · GitHub Actions

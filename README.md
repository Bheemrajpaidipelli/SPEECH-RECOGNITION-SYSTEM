# SPEECH-RECOGNITION-SYSTEM
COMPANY : CODTECH IT SOLUTIONS NAME : PAIDIPELLI BHEEMRAJ ID : CT06DF373 DOMAIN : ARTIFICIAL INTELLIGENCE DURATION : 6 WEEKS MENTOR : NEELA SANTHOSH KUMAR
Speech-to-Text Grammar Corrector

Overview:
---------
This project captures spoken input from a microphone, transcribes it using Google Speech Recognition,
and then automatically corrects grammar, punctuation, and sentence structure using LanguageTool.
It is a simple, effective tool for generating grammatically correct text from voice input.

Key Features:
-------------
- Real-time voice capture using your microphone
- Transcription using Google's Speech Recognition API
- Grammar and punctuation correction using LanguageTool
- Sentence formatting with proper capitalization and final punctuation
- Friendly feedback for silence, misrecognition, or errors

Technologies Used:
------------------
- Python 3.7+
- SpeechRecognition
- PyAudio
- language_tool_python
- Regular expressions (re)

Installation Instructions:
--------------------------
1. Make sure Python 3 is installed on your system.

2. Install the required libraries using pip:
   pip install SpeechRecognition pyaudio language-tool-python

   Note: If PyAudio fails to install (common on Windows), download the correct wheel file (.whl) from:
   https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyaudio
   Then install it manually:
   pip install PyAudio‑0.2.11‑cp311‑cp311‑win_amd64.whl

How to Run:
-----------
1. Ensure your microphone is plugged in and accessible.
2. Run the script:
   python speech_corrector.py
3. When prompted with "Ready. Speak now...", begin speaking.
4. The system will:
   - Capture your voice
   - Transcribe the spoken text
   - Correct the grammar and format the output
5. The final output will be printed in a clean, correct form.

Example:
--------
You say:     "i go to school every day but not yesterday"
Raw:         i go to school every day but not yesterday
Corrected:   I go to school every day but not yesterday.

Error Handling:
---------------
- If you don’t speak in time → "You didn’t start speaking in time."
- If speech is unclear → "Speech detected, but not understood."
- If Google STT fails → "API error: <details>"

Use Cases:
----------
- Practicing spoken English
- Voice-to-text apps with grammar support
- Accessibility tools for speech transcription
- Grammar correction in voice interfaces

Tips:
-----
- Speak clearly and naturally.
- Ensure a quiet environment for best accuracy.
- Change the 'seed_text' or timeout parameters in code to adjust behavior.

Credits:
--------
- SpeechRecognition: https://pypi.org/project/SpeechRecognition/
- LanguageTool: https://github.com/languagetool-language-server/language-tool-python
- Dataset: Your own voice via microphone

License:
--------
This project is licensed under the MIT License.

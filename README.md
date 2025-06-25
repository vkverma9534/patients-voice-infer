# patients-voice-infer
Patients Voice Infer is a tool that helps extract patient info just from their voice. It takes the speech, converts it to text and try to find name, age, gender and symptoms. Then based on what patient said, it decides which doctor is best for them.
The project inputs the voice of patient using sounddevice (python library).The voice is saved via an autorefreshing .wav file then the file is transcribed using Openai Whisper. The raw transcription then passed to an AI function which extracts the desirable data into desirable format. This allows proper saving of information, before registering the patient we confirm the credential if correct we provide them with a token number (which auto-updates if the patient is successfully registered).
At this very moment we use another AI integrated function which analyses patient's symptoms and provide them with the appropriate doctor on that basis.
Once all the above steps are completed the information gets saved into seperate directory of specific doctor.
In the meantime a directory of a patient is maintained which holds all patient we use the directory on patient display , so that all patients keep track of their status.

## TOOLS USED
a) Sounddevice --> records voice.
b) Openai Whisper --> Transcribes the sound (voice to text).
c) Mistral (llama) --> AI used for data extraction and doctor assignment.
d) Pandas --> Used for creating Data frames.

!!YOU MIGHT NEED TO INSTALL THE REQUIRED LIBRARIES AND APIs TO MAKE THE PROJECT FUNCTIONAL ON YOUR DEVICE!!

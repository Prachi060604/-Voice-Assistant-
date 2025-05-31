# -Voice-Assistant-
 Voice Assistant using Python in Jupiter Notebook




pip install pyttsx3

pip install wikipedia

import pyttsx3
import wikipedia

# let name of your assistance will voice

voice=pyttsx3.init()
In=input("Search Wikipedia/Google: ")
result=wikipedia.summary(In,sentences=2)
print(result)
voice.say(result)
voice.runAndWait()

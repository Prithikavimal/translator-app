# translator-app
pip install googletrans==4.0.0-rc1
from googletrans import Translator

def translate_text(text, dest_lang='en'):
    translator = Translator()
    translated_text = translator.translate(text, dest=dest_lang)
    return translated_text.text

if __name__ == "__main__":
    text = input("Enter the text to translate: ")
    dest_lang = input("Enter the destination language (e.g., 'fr' for French, 'es' for Spanish): ")

    translated_text = translate_text(text, dest_lang)
    print("Translated text:", translated_text)

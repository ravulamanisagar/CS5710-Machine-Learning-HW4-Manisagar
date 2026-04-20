import spacy

# Load English model
nlp = spacy.load("en_core_web_sm")

# Input text
text = "John enjoys playing football while Mary loves reading books in the library."

# Process text
doc = nlp(text)

# Step 1: Tokenization
tokens = [token.text for token in doc]
print("Tokens:", tokens)

# Step 2–4: Remove stopwords, lemmatize, keep nouns & verbs
filtered_words = []

for token in doc:
    if not token.is_stop:  # remove stopwords
        if token.pos_ in ["NOUN", "VERB"]:  # keep only nouns & verbs
            filtered_words.append(token.lemma_)  # lemmatization

print("Final Output:", filtered_words)



# utsbigdata
import nltk 
import string   
kalimat = "Saya Bangga jadi warga nahdlatul ulama." 
kalimat = kalimat.translate(str.maketrans('','',string.punctuation)).lower()   
tokens = nltk.tokenize.word_tokenize(kalimat) 
kemunculan = nltk.FreqDist(tokens) 
print(kemunculan.most_common())

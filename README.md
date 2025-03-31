# Surprisal of VPs and Case-Marked NPs in Japanese
This is part of an individual research project for LIGN 169: Information Theory at UCSD. This project will explore the average surprisal of verb phrases (VPs), and the average surprisal of case-marked NPs, both in Japanese. Additionally, we will compare these with these same surprisals in English to identify a unique property of Japanese grammar.

The project first needs a treebank that needs to be parsed through. To analyze the data, I've imported the Japanese-PUD treebank to parse through and extract phrases and find surprisal values. The PUD (Parallel-Universal Dependencies) files is especially great for comparing values of two languages, as it uses the same sentences cross-linguistically. I've used the PUD treebank instead of Japanese-GSD is to later compare the surprisals of Japanese and English to see if there is anything greater to uncover about sentence processing using surprisal.

Note: This treebank is written in Kanji

## Case-marked NP Surprisal
Japanese uses a very detailed case marking system. For the project, we will look at nominative (NOM), accusative (ACC), dative (DAT), and genitive (POSS). These markers in Japanese are が 'ga', を 'wo', に 'ni', and の: 'no' respectively.  The function below will compute the average surprisal values for these three case markers, starting by taking in nouns from a treebank, finding its dependents to create NPs, and calculating the surprisal, on average, of these NPs depending on their case.

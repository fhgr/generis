# Deep Learning and Background Knowledge for Named Entity Recognition

Unter Named Entity Recognition (NER) versteht man ein Text Analyseverfahren, welches automatisch Nennungen von benannten Entitäten (zum Beispiel Personen, Lokationen und Organisationen) in Text identifiziert. Im Gegensatz zum Named Entity Linking (NEL) wird dabei nur der Entitätstyp _nicht_ jedoch die eigentliche Entität (zum Beispiel um welche Person es sich handelt) erkannt.
Text Analytics Verfahren verwenden die identifizierten Entitäten in Folge für die Erweiterung von Wissensbasen und um automatisch Kontextinformation (z.B. Produkte und Services einer Firma, zugehörige Adressinformation, etc.) zu den erkannten Entitäten zu sammeln.
NER stellt daher eine wichtige Schlüsseltechnologie für den Aufbau von Knowledge und Information Extraction Techniken dar. Populäre bestehende Ansätze, wie zum Beispiel der Stanford NER Tagger und AllenNLP setzen zwar teilweise bereits Deep-Learning Techniken ein, verzichten aber vollständig auf Hintergrundwissen, um diese zu trainieren beziehungsweise um deren Genauigkeit zu verbessern.


## Vorhandene Ressourcen

* Standardisierte Corpora für das Training und die Evaluation von NER Komponenten
* Hintergrundwissen, welches im Rahmen des Job-Cockpit Projektes erstellt wurde bzw. als Linked Open Data zur Verfügung steht:
    - Listen von Vor- und Nachnamen welche häufig in den .us/.gb/.ch verwendet werden.
    - Geographische Lokationen (geonames.org)
    - Listen von Organisationen und Firmen (wikidata).
    - Ontologien, welche domänen-spezifisches Wissen codieren

## Ziele

 1. Kurzer Überblick über bestehende Verfahren
 2. Implementierung: Es soll ein NER Tagger für die in den Projekten relevanten Named Entities entwickelt werden. 
    - Ausgangsbasis: ausgewählte Ansätze aus der Literatur 
    - Integration von Hintergrundwissen, welches für das Training und/oder das Tagging verwendet werden soll
 4. Evaluierung: Basierend auf Standard Evaluationskorpora mittels der Metriken Precision/Recall/F1 (vergleiche [Orbis](https://github.com/orbis-eval/orbis_eval).


## Starting points:

* Li,J., A. Sun, J. Han, and C. Li. “A Survey on Deep Learning for Named Entity Recognition.” IEEE Transactions on Knowledge & Data Engineering, no. 01 (March 2020): 1–1. https://doi.org/10.1109/TKDE.2020.2981314.
* Stanford NER Tagger (https://nlp.stanford.edu/software/CRF-NER.shtml)
* Xie, Jiateng, Zhilin Yang, Graham Neubig, Noah A. Smith, and Jaime G. Carbonell. “Neural Cross-Lingual Named Entity Recognition with Minimal Resources.” In EMNLP, 2018. https://doi.org/10.18653/v1/d18-1034.
* AllenNLP (https://allennlp.org/)
* Stanford Stanza (https://github.com/stanfordnlp/stanza)

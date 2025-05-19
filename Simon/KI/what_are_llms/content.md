---
title: "Was sind eigentlich LLMs – und warum reden gerade alle darüber?"
author: "Simon Sterneder"
date: 2025-05-19
reading_time: "3 min"
---

# Was sind eigentlich LLMs – und warum reden gerade alle darüber?

**L**arge **L**anguage **M**odels wie ChatGPT sind in kürzester Zeit zu einem festen Bestandteil meines Arbeitsalltags geworden. Als Entwickler nutze ich sie inzwischen regelmäßig – beim Debugging, beim Refactoring, zum Schreiben von Dokumentation oder um neue Frameworks schneller zu verstehen. Was vor Kurzem noch wie ein spannendes Experiment wirkte, ist heute ein praktisches Werkzeug, das mir Zeit spart, Ideen liefert und manchmal sogar neue Denkansätze eröffnet.

Und ich bin damit nicht allein. In Büros, Schulen und Medien sind LLMs wie ChatGPT, Claude oder Gemini derzeit in aller Munde. Die einen feiern sie als Durchbruch in Sachen Produktivität und Kreativität, die anderen warnen vor Fehlinformationen, Urheberrechtsproblemen oder ethischen Grauzonen.

In diesem Artikel will ich verständlich erklären:
- was LLMs eigentlich sind – und wie sie funktionieren,
- wie sie sich von anderen KI-Systemen unterscheiden,
- wo sie aktuell sinnvoll eingesetzt werden,
- welche Risiken und Herausforderungen es gibt,
- und was in Zukunft technisch und gesellschaftlich auf uns zukommt.

Egal ob du selbst entwickelst, dich für KI interessierst oder einfach verstehen willst, was hinter dem Hype steckt – hier bekommst du einen kompakten Überblick.

## Inhalt
1. KI kurz erklärt – und wo LLMs ins Bild passen
2. LLMs im Alltag – was sie können und wie sie wirken
3. Wie LLMs entstanden sind – ein Blick zurück
4. Wie LLMs unter der Haube funktionieren
5. Überblick: Die wichtigsten LLMs im Vergleich
6. LLMs im echten Leben – was schon geht
7. Risiken & Grenzen
8. Regulierung & Verantwortung
9. Wohin geht die Reise? Drei Zukunftsszenarien

## 1. KI kurz erklärt – und wo LLMs ins Bild passen
Wenn heute von „KI“ die Rede ist, denken viele sofort an Chatbots oder Bildgeneratoren. Dabei ist Künstliche Intelligenz (KI) ein deutlich breiteres Feld. Grob gesagt geht es darum, Maschinen mit Fähigkeiten auszustatten, die wir sonst mit menschlicher Intelligenz verbinden: Lernen, Problemlösen, Muster erkennen, Entscheidungen treffen.

LLMs sind ein Teilbereich dieser großen KI-Welt – genauer gesagt gehören sie zur sogenannten "generativen KI", also zu Systemen, die Inhalte erzeugen können: Texte, Bilder, Code oder sogar Musik. Doch bevor wir uns LLMs im Detail anschauen, lohnt ein kurzer Blick aufs große Ganze.

### KI ist nicht gleich KI: Ein kurzer Überblick

Neben Sprachmodellen wie ChatGPT gibt es viele weitere Arten von KI-Systemen. Einige Beispiele:

**Computer Vision:** Hier geht’s um das Erkennen und Verstehen von Bildern oder Videos. Klassische Anwendungen sind Gesichtserkennung oder Objektdetektion in der Industrie.

**Reinforcement Learning:** Diese Technik bringt Maschinen bei, durch Versuch und Irrtum besser zu werden – ähnlich wie ein Kind, das Fahrradfahren lernt.

**Symbolische KI & regelbasierte Systeme:** Diese „klassischen“ KI-Ansätze basieren nicht auf Daten, sondern auf festgelegten Regeln.

### Wo LLMs ins Bild passen

LLMs (Large Language Models) gehören zum Natural Language Processing (NLP) – also zur Verarbeitung natürlicher Sprache. Anders als frühere NLP-Systeme, die oft stark regelbasiert oder auf spezifische Aufgaben trainiert waren, können moderne LLMs flexibel auf unterschiedlichste Eingaben reagieren.

Ihr Erfolg beruht auf einem zentralen Fortschritt: Statt Sprache Wort für Wort zu verstehen, lernen sie auf Basis riesiger Textmengen, Wahrscheinlichkeiten für die nächsten Wörter vorherzusagen – ein Ansatz, der erstaunlich gut funktioniert.

## 2. LLMs im Alltag – was sie können und wie sie wirken

LLMs sind erstaunlich vielseitig. Ein und dasselbe Modell kann auf völlig unterschiedliche Aufgaben reagieren – je nachdem, wie es angesprochen wird. Hier ein paar Beispiele aus dem Alltag:

**Als Entwicklerhilfe:** Debugging, Code-Optimierung, Dokumentation, Framework-Training

**Als Sprachlehrer:** Erklärungen, Beispielsätze, Vokabeltraining

**Als Recherchetool:** Faktenchecks, Themenüberblicke, Zusammenfassungen

**Als Ideengeber:** Strukturentwürfe, Schreibimpulse, Namensvorschläge

Der Schlüssel ist: LLMs brauchen keine vordefinierten Befehle. Stattdessen reagieren sie flexibel auf Spracheingaben – das sogenannte Prompting.

### Wie das funktioniert – ein kurzes Beispiel

Technisch basiert ein LLM auf einem Transformer-Modell, das Muster erkennt und sinnvolle Fortsetzungen berechnet. Sprache wird in Tokens zerlegt, in Zahlen umgewandelt und dann statistisch bewertet.

**Beispiel:** Ein Prompt – viele Talente

``` text
Prompt: "Erkläre mir, wie Merge Sort funktioniert – in einfachen Worten, mit Beispielcode in Python."

Antwort: (verkürzt)
Merge Sort ist ein sogenannter Divide-and-Conquer-Algorithmus. Das bedeutet, dass das Problem in kleinere Teile zerlegt wird, die dann einzeln gelöst und wieder zusammengesetzt werden. (...)

Python-Code:
def merge_sort(arr):
    if len(arr) <= 1:
        return arr
    ...
```

Je nach Formulierung des Prompts kann das Modell hier auch eine anschauliche Analogie liefern („Stell dir vor, du sortierst Spielkarten…“) oder den Code kommentieren, debuggen oder umschreiben.

## 3. Wie LLMs entstanden sind – ein Blick zurück

LLMs sind das Ergebnis jahrelanger Forschung. Seit dem Transformer-Durchbruch 2017 ging es rasant voran:
- **GPT-2** (2019): ~1,5 Mrd. Parameter
- **GPT-3** (2020): 175 Mrd. Parameter
- **GPT-4** (2023): Größe unbekannt, aber deutlich leistungsstärker

Parallel entstanden leistungsfähige Open-Source-Modelle:
- LLaMA 3 (Meta), Mistral, Falcon, BLOOM u. a.

### Wie groß ist "groß"?

**GPT-3** > 86 Mrd. Neuronen im menschlichen Gehirn

Millionen $ Rechenkosten, hoher Strombedarf, CO₂-Ausstoß

**Aber:** Größe allein ist nicht alles. Architektur, Datenqualität und Feintuning spielen ebenso eine Rolle.

## 4. Wie LLMs unter der Haube funktionieren
### Tokenisierung

Text wird in Tokens zerlegt und in Zahlen umgewandelt. Beispiel:
```
"ChatGPT erklärt Code." → ["Chat", "G", "PT", " erklärt", " Code", "."] 
```

### Embeddings
Tokens werden in Vektorräume eingebettet – Bedeutungsnähe wird mathematisch erfassbar.

### Attention – wer spricht mit wem?

Self-Attention ermöglicht Kontextverständnis. Beispiel:
```
1. Der Hund hat den Mann gebissen.
2. Der Mann hat den Hund gebissen.
```
Gleiche Wörter, andere Reihenfolge – andere Bedeutung. Attention erkennt solche Rollenunterschiede.

### Training vs. Inferenz

- **Training:** Wochenlange Berechnungen mit riesigen Datenmengen
- **Inferenz:** Reaktion in Echtzeit auf Nutzereingaben

### Ressourcen

- Hoher Stromverbrauch, tausende GPUs, spezialisierte Rechenzentren
- Milliarden Tokens im Training

## 5.Überblick: Die wichtigsten LLMs im Vergleich

| Modell      | Offenheit         | Kontextgröße | Multimodal? | Fokus           | Quellenangabe |
|-------------|-------------------|---------------|-------------|------------------|----------------|
| ChatGPT     | Proprietär        | Hoch          | Ja          | Vielseitigkeit   | Teilweise       |
| Gemini      | Proprietär        | Sehr hoch     | Ja          | Fakten + Code    | Teilweise       |
| Claude      | Proprietär        | Sehr hoch     | (Bald)      | Sicherheit       | Nein            |
| LLaMA       | Open-Weight       | Mittel        | Nein        | Forschung        | Nein            |
| Copilot     | Proprietär        | Hoch          | Teilweise   | Produktivität    | Nein            |
| Perplexity  | Teilweise offen   | Mittel        | Nein        | Webrecherche     | Ja              |

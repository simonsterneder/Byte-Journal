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

**Prompt:** <br>
<code> "Erkläre mir, wie Merge Sort funktioniert – in einfachen Worten, mit Beispielcode in Python."</code>

**Antwort (gekürzt):**
### 🧠 Was ist Merge Sort?
Merge Sort ist ein "Teile und Herrsche" (Divide and Conquer)-Algorithmus zum Sortieren von Listen. Das bedeutet:

Teilen: Zerteile die Liste in zwei Hälften.

Sortieren: Sortiere jede Hälfte rekursiv (also nach dem gleichen Prinzip).

Zusammenfügen (Merge): Füge die beiden sortierten Hälften so zusammen, dass die gesamte Liste sortiert ist.

### 📊 Beispiel: Liste [5, 3, 8, 6, 2, 7, 4, 1]
Zerlege in Hälften: 
```python 
[5, 3, 8, 6]  [2, 7, 4, 1]
``` 

Zerlege weiter, bis nur noch Einzellisten da sind:
```python 
[5], [3], [8], [6], [2], [7], [4], [1]
``` 

Jetzt Merge:
```python 
[5] + [3] → [3, 5]  
[8] + [6] → [6, 8]
``` 

usw., bis am Ende:
```python 
[1, 2, 3, 4, 5, 6, 7, 8]
``` 

### 🧑‍💻 Python-Code
```python
def merge_sort(arr):
    # Wenn die Liste 0 oder 1 Element hat, ist sie schon sortiert
    if len(arr) <= 1:
        return arr

    # Liste in zwei Hälften teilen
    mid = len(arr) // 2
    left_half = merge_sort(arr[:mid])
    right_half = merge_sort(arr[mid:])

    # Die sortierten Hälften zusammenführen
    return merge(left_half, right_half)

def merge(left, right):
    sorted_list = []
    i = j = 0

    # Solange beide Listen noch Elemente haben
    while i < len(left) and j < len(right):
        if left[i] < right[j]:
            sorted_list.append(left[i])
            i += 1
        else:
            sorted_list.append(right[j])
            j += 1

    # Restliche Elemente anhängen (nur eine Liste hat noch was übrig)
    sorted_list.extend(left[i:])
    sorted_list.extend(right[j:])

    return sorted_list

# Beispiel:
unsortierte_liste = [5, 3, 8, 6, 2, 7, 4, 1]
sortierte_liste = merge_sort(unsortierte_liste)
print(sortierte_liste)
```

### 🟢 Ausgabe:
```python 
[1, 2, 3, 4, 5, 6, 7, 8]
```

### ✅ Vorteile von Merge Sort:
- Sehr effizient: immer 𝑂(𝑛 log 𝑛)
- Funktioniert auch gut bei großen Datenmengen
- Stabiler Sortieralgorithmus (Reihenfolge bleibt bei gleichen Werten erhalten)

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

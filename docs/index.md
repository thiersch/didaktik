---
Title: Konstruktive Unterstützung
sidebar_position: 1
---


# Konstruktive Unterstützung im Unterricht

Konstruktive Unterstützung beschreibt professionelles Lehrkräftehandeln, das Lernende **fachlich, emotional und strategisch** so begleitet, dass sie Aufgaben **zunehmend selbstständig** bewältigen können. Sie ist eng verbunden mit **positiver Fehlerkultur**, **Scaffolding** und **lernprozessbezogenem Feedback**.

Diese Seite richtet sich an **Lehrkräfte und angehende Lehrkräfte** und führt praxisnah in das Thema ein – mit Beispielen aus dem **(Informatik-/Webentwicklungs-)Unterricht**, Übungen und Quizzes.

---

## Warum konstruktive Unterstützung?

Gerade in anspruchsvollen Lernbereichen (z. B. Programmieren, Problemlösen, Modellieren) zeigen sich typische Risiken:

* Überforderung durch Komplexität
* Frustration bei Fehlern
* Rückzug oder bloßes Abschreiben

➡ Konstruktive Unterstützung zielt darauf ab,

* Lernprozesse **sichtbar** zu machen,
* Fehler **lernwirksam** zu nutzen,
* und die **Selbstwirksamkeit** der Lernenden zu stärken.

---

## Zentrale Bausteine konstruktiver Unterstützung

<Columns>
  <Column className="text--left">
    ### Beziehung & Lernklima
    Lernende erleben Fehler als erlaubt und sinnvoll.

```
*Beispiel:* „Der Fehler hilft uns zu verstehen, wie der Code denkt.“
```

  </Column>
  <Column className="text--left">
    ### Diagnose
    Die Lehrkraft interessiert sich für Denkwege, nicht nur für Ergebnisse.

```
*Beispiel:* „Was war deine Idee hinter dieser Lösung?“
```

  </Column>
  <Column className="text--left">
    ### Scaffolding
    Unterstützung wird **gestuft** angeboten und wieder zurückgenommen.

```
*Beispiel:* Leitfrage → Codegerüst → Erklärung
```

  </Column>
</Columns>

---

## Fehler als Lernanlass verstehen

Nicht jeder Fehler ist gleich – für konstruktive Unterstützung ist die **Einordnung entscheidend**.

* **Fachlicher Fehler:** Fehler in Logik, Syntax, Anwendung
* **Lernprozess-Fehler:** notwendiger Zwischenschritt im Denken
* **Bewertungsfehler:** entsteht durch unangemessene Rückmeldung der Lehrkraft

---

<details>
  <summary>Übung 1: Fehler einordnen</summary>

<ItemMatch taskData={[
{ id: 'f1', text: 'Die if-Bedingung wird nie wahr.', answer: 'Fachlicher Fehler' },
{ id: 'f2', text: 'Client- und Serverlogik werden vermischt.', answer: 'Lernprozess-Fehler' },
{ id: 'f3', text: '„Das kannst du doch eigentlich.“', answer: 'Bewertungsfehler' },
{ id: 'f4', text: 'SQL-INSERT ohne Feldliste.', answer: 'Fachlicher Fehler' },
]} />

</details>

---

## Lehrkraftsprache: produktiv oder unproduktiv?

Sprache ist eines der **wirksamsten Werkzeuge** konstruktiver Unterstützung.

* **Produktiv:** lernprozessbezogen, wertschätzend, aktivierend
* **Unproduktiv:** bewertend, pauschalisierend, demotivierend

---

<details>
  <summary>Übung 2: Aussagen bewerten</summary>

<ItemMatch taskData={[
{ id: 'a1', text: 'Die Struktur stimmt, prüfe nochmal die Bedingung.', answer: 'produktiv' },
{ id: 'a2', text: 'Das ist falsch, das hatten wir schon.', answer: 'unproduktiv' },
{ id: 'a3', text: 'Interessanter Ansatz – was passiert im Randfall?', answer: 'produktiv' },
{ id: 'a4', text: 'Das ist zu kompliziert für dich.', answer: 'unproduktiv' },
]} />

</details>

---

## Scaffolding: Hilfe dosieren

Konstruktive Unterstützung bedeutet nicht, sofort zu erklären, sondern **gezielt Hilfe anzubieten**:

<Columns>
  <Column className="text--left">
    **Niedrig**  
    Diagnostische Fragen
  </Column>
  <Column className="text--left">
    **Mittel**  
    Strukturhilfen, Gerüste
  </Column>
  <Column className="text--left">
    **Hoch**  
    Modellieren, explizite Erklärung
  </Column>
</Columns>

---

<details>
  <summary>Übung 3: Hilfestellungen einordnen</summary>

<ItemMatch taskData={[
{ id: 'h1', text: 'Was erwartest du an dieser Stelle im Ablauf?', answer: 'produktiv' },
{ id: 'h2', text: 'Ich mache das jetzt schnell für dich.', answer: 'unproduktiv' },
{ id: 'h3', text: 'Nutze das Gerüst und ergänze die fehlende Logik.', answer: 'produktiv' },
{ id: 'h4', text: 'Das liegt dir einfach nicht.', answer: 'unproduktiv' },
]} />

</details>

---

## Wissen überprüfen: Quiz

<details>
  <summary>Bereit für das Quiz?</summary>

<Quiz questions={[
{
question: 'Welche Aussage fördert Selbstkorrektur am stärksten?',
answers: [
{ text: 'Das ist falsch.', isCorrect: false },
{ text: 'Wann wird deine Bedingung eigentlich wahr?', isCorrect: true },
{ text: 'So geht das nicht.', isCorrect: false },
{ text: 'Ich erkläre es dir nochmal komplett.', isCorrect: false }
],
},
{
question: 'Warum sind Fehler besonders lernwirksam?',
answers: [
{ text: 'Weil sie benotet werden.', isCorrect: false },
{ text: 'Weil sie Denkprozesse sichtbar machen.', isCorrect: true },
{ text: 'Weil sie vermieden werden müssen.', isCorrect: false },
{ text: 'Weil sie Zeit sparen.', isCorrect: false }
],
},
{
question: 'Was widerspricht konstruktiver Unterstützung?',
answers: [
{ text: 'Diagnostische Fragen stellen', isCorrect: false },
{ text: 'Fehler entpersonalisieren', isCorrect: false },
{ text: 'Fehler öffentlich abwerten', isCorrect: true },
{ text: 'Scaffolding einsetzen', isCorrect: false }
],
},
{
question: 'Wann ist hohe Unterstützung sinnvoll?',
answers: [
{ text: 'Bei jeder Aufgabe', isCorrect: false },
{ text: 'Wenn Lernende völlig orientierungslos sind', isCorrect: true },
{ text: 'Wenn Lernende selbstständig arbeiten', isCorrect: false },
{ text: 'Zur Leistungsbewertung', isCorrect: false }
],
},
]} />

</details>

---

## Merksatz

> *Konstruktive Unterstützung zeigt sich nicht im schnellen Erklären, sondern im professionellen Begleiten von Lernprozessen.*

---
Title: Konstruktive Unterstützung
sidebar_position: 1
---


# Konstruktive Unterstützung im Unterricht

Konstruktive Unterstützung beschreibt professionelles Lehrkräftehandeln, das Lernende **fachlich, emotional und strategisch** so begleitet, dass sie Aufgaben **zunehmend selbstständig** bewältigen können. Sie ist eng verbunden mit **positiver Fehlerkultur**, **Scaffolding** und **lernprozessbezogenem Feedback**.


---

## Ziel: Selbstständige Entwicklung

Das Ziel konstruktiver Unterstützung ist es, die **selbstständige Entwicklung** der Lernenden zu fördern. Konstruktive Unterstützung wird ermöglich durch

* Positive Beziehung zu den Lernenden
* Formatives Assessment und Feedback
* Positive Fehlerkultur
* Dosierte, abgestufte Hilfestellung (Scaffolding)


## Zone der nächsten Entwicklung
Wirksames Lernen findet in der Zone zwischen Unterforderung und Überforderung statt. Die konstruktive Unterstützung soll Lernen in dieser Zone ermöglichen. [Text ausarbeiten]

export const Zone = ({ title, subtitle, isCenter }) => (
  <div style={{
    flex: 1,
    padding: '20px',
    textAlign: 'center',
    display: 'flex',
    flexDirection: 'column',
    justifyContent: 'center',
    border: isCenter ? '2px solid white' : 'none',
    margin: isCenter ? '4px' : '0',
    borderRadius: '4px'
  }}>
    <div style={{ fontWeight: 'bold', fontSize: '1.1rem', marginBottom: '8px' }}>{title}</div>
    <div style={{ fontSize: '0.9rem' }}>{subtitle}</div>
  </div>
);


<div style={{ width: '100%', fontFamily: 'sans-serif', margin: '2rem 0' }}>
  <div style={{
    display: 'flex',
    minHeight: '200px',
    borderRadius: '8px',
    overflow: 'hidden',
    color: 'black',
    background: 'linear-gradient(to right, #82ada9, #e9c46a, #e76f51)'
  }}>
    <Zone 
      title="Unterforderung" 
      subtitle="Aufgaben können selbstständig ohne Hilfe bewältigt werden." 
    />
    <Zone 
      title="Zone der nächsten Entwicklung" 
      subtitle="Aufgaben können mit Unterstützung anderer bewältigt werden."
      isCenter={true}
    />
    <Zone 
      title="Überforderung" 
      subtitle="Aufgaben können auch mit Hilfe anderer nicht bewältigt werden." 
    />
  </div>
  <div style={{ textAlign: 'center', marginTop: '10px', fontSize: '0.8rem', fontStyle: 'italic' }}>
    ◀ —————————————————— Aufgabenschwierigkeit —————————————————— ▶
  </div>
</div>

---

## Alltägliche Situation in Klassenzimmern



Die alltägliche Situation in Klassenzimmern zeigt oftmals ein diffuses Bild. Neben unterforderten Lernenden gibt es Überforderte, die eventuell viel Zeit der Lehrkraft benötigen. Daneben ist es typisch, dass sich Lösungen in Sitzreihen ausbreiten und es schwierig zu bestimmen ist, wo ihr Ursprung liegt. Dazu gibt es "unbekannte" Inseln, die schwer erreichbar sind oder an denen Personen sitzen, die der Lehrkraft nicht auffallen.
![Im Klassenzimmer hat jeder eine eigene Lernzone](./klassenzimmer_baeren.png)

---


## Zentrale Bausteine konstruktiver Unterstützung

<Columns>
  <Column className="text--left">
    ### Beziehung & Lernklima
    Lernende erleben Fehler als erlaubt und sinnvoll.


*Beispiel:* „Der Fehler hilft uns zu verstehen, wie der Code denkt.“


  </Column>
  <Column className="text--left">
    ### Diagnose
    Die Lehrkraft interessiert sich für Denkwege, nicht nur für Ergebnisse.


*Beispiel:* „Was war deine Idee hinter dieser Lösung?“


  </Column>
  <Column className="text--left">
    ### Scaffolding
    Unterstützung wird **gestuft** angeboten und wieder zurückgenommen.


*Beispiel:* Leitfrage → Codegerüst → Erklärung


  </Column>
</Columns>

---

## Fehler als Lernanlass verstehen

Nicht jeder Fehler ist gleich – für konstruktive Unterstützung ist die **Einordnung entscheidend**.

Typische Fehler Lernender:
* **Fachlicher Fehler:** Fehler in Logik, Syntax, Anwendung
* **Lernprozess-Fehler:** notwendiger Zwischenschritt im Denken

Typische Fehler Lehrender:

* **Bewertungsfehler:** entsteht durch unangemessene Rückmeldung der Lehrkraft

---

<details>
  <summary>Übung 1: Fehler von Lehrenden und Lernenden einordnen</summary>

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

:::info[Merke]


Scaffolding ist die gerade richtig dosierte Begleitung selbstbestimmten Lernens.

:::

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

---

# Medical Dashboard

A React dashboard for reviewing patient records, built as a university project for a
human-computer interaction course.

## What it does

The app opens on a dashboard, with a sidebar for moving between pages. Patients are
clickable wherever they appear and each one leads to their own detail page.

**Patient detail** is built around a timeline of the patient's history. Clicking a point
on it opens an overlay with the full event. The coloured buttons above the timeline
("Medikament", "Lab", and so on) work as both a legend and a filter, and the visible range
can be narrowed by date. "Add Event" adds a new entry, which appears on the timeline
straight away.

**Notes** are split into previous notes and a new note. Anything typed is held if you
navigate away before saving, and saved notes can be reopened, edited or deleted.

**Overview** tracks the most recent diagnoses, medications and allergies, and new
allergies can be added inline.

## Running it

```bash
npm install
npm run dev
```

Patient data ships as static JSON files, so there is no backend to set up.

Built with React, Vite and Recharts, with react-router-dom for routing and
react-datepicker for date input.

---

*The original German documentation follows.*

# Anweisungen zur Installation:
1. Die Daten sind in JSON-Dateien im Projekt enthalten. Notwendige Module können mit npm install installiert werden. Die App kann mit npm run dev gestartet werden.
2. Alternativ können die Module mit folgenden Befehlen installiert werden:
- npm install react-router-dom
- npm install recharts
- npm install react-datepicker

# Nutzung
### Dashboard:
Das Programm startet im Dashboard. Über die Sidebar auf der linken Seite kann zu den anderen Seite navigiert werden. Auf allen Seiten können die Patienten angeklickt werden, damit navigiert man zur entsprechenden Patientendetailseite. Auf dem Dashboard kann dafür auch die Komponente "Next Patient Details" angeklickt werden.

### Patientendetailseite:
In der Mitte der Patientendetailseite gibt es eine Timeline zur Darstellung der Patientenhistorie. Werden die Punkte in der Timeline angeklickt öffnet sich ein Overlay mit Details. Die Buttons "Medikament", "Lab", etc. stellen die Legende der Farben dar und können auch angeklickt werden zum Filtern. Genauso kann der Anzeigebereich mit Eingabe eines Datums gefiltert werden. Über "Add Event" können neue Daten hinzugefügt werden, diese erscheinen als Punkt auf der Timeline.

### Notizen:
Die Notizen sind in zwei Felder unterteilt, auf der linken Seite Previous Notes und auf der rechten Seite New Note. Es können neue Notizen eingegeben werden, diese werden automatisch zwischengespeichert, falls die Seite verlassen wird. Mit dem Save Note Button, werden die Notizen gespeichert und erscheinen auf der linken Seite. Die Notizen können in der Liste angeklickt und im neuen Overlay angesehen, bearbeitet oder gelöscht werden.

### Overview:
Das Overview auf der rechten Seite zeigt dynamisch die aktuellsten Diagnosen, Medikationen und Allergien an. Es können neue Allergien mit Klick auf den + Button hinzugefügt werden. 

# Dateistruktur
- assets/:  Beinhaltet Bilder, die wir benutzt haben, z.B. Arzt, Patient.
- components/: Beinhaltet  wiederverwendbare React-Komponenten wie Tabellen, Diagramme und Filter.
- data/: Enthält statische JSON-Dateien, die Daten wie Termine, Patienteninformationen und Medikationspläne simulieren.
- pages/: Hauptseiten der Anwendung, darunter App.jsx und die globale Initialisierung in main.jsx.

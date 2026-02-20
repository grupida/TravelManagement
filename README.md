# ✈️ TravelHub

**Effizienter Reisemanagement-Prozess ohne Selbstbuchung**

TravelHub ist eine Single-Page-Anwendung für das zentrale Management von Dienstreisen. Mitarbeitende stellen Anfragen, das Travel Desk erstellt Optionen, und der Workflow wird digital abgebildet.

---

## 🚀 Features

### Mitarbeiter-Modus
- ✅ **Reiseanfrage-Formular** - Umfassender Fragebogen für alle Anforderungen
- ✅ **Anfragen-Übersicht** - Status-Tracking aller eigenen Reisen
- ✅ **Optionen ansehen** - Hotel-Optionen (A/B/C) vergleichen und auswählen
- ✅ **Freigabe** - Ein-Klick-Bestätigung der gewählten Option

### Travel Desk-Modus
- ✅ **Dashboard** - Übersicht aller Anfragen nach Status
- ✅ **Workflow-Management** - Eingegangen → Bearbeitung → Optionen → Freigabe → Gebucht
- ✅ **Optionen erstellen** - Bis zu 3 Hotel-Optionen mit Preisen dokumentieren
- ✅ **Buchungsabschluss** - Bestätigungscode erfassen
- ✅ **Filter & Suche** - Schnelles Finden von Anfragen

---

## 📋 Workflow

```
1. Mitarbeiter → Reiseanfrage stellen (Formular)
2. Travel Desk → Anfrage in Bearbeitung nehmen
3. Travel Desk → Hotel-Optionen (A/B/C) erstellen & senden
4. Mitarbeiter → Option auswählen & freigeben
5. Travel Desk → Buchung abschließen & Bestätigung erfassen
```

---

## 🛠 Tech-Stack

- **Frontend:** HTML5, CSS3, JavaScript (Vanilla)
- **Database:** sql.js (SQLite im Browser)
- **Storage:** localStorage (lokale Persistenz)
- **Deployment:** GitHub Pages ready

---

## 🎯 MVP Scope

**✅ In Scope:**
- Reiseanfrage-Formular mit allen Basis-Anforderungen
- Hotel-Optionen (A/B/C) Management
- Status-Tracking (submitted → booked)
- Mitarbeiter- & Travel Desk-Modus

**🔮 Geplant für Phase 2:**
- Rechnungsmanagement & 3-Way-Match
- Auslagen per Foto (OCR)
- ProCos Integration (Stammdaten)
- Flug/Zug-Buchung (Ausland)
- Backend & Multi-User

---

## 🚀 Schnellstart

1. **Lokal starten:**
   ```bash
   # Einfach index.html im Browser öffnen
   open index.html
   ```

2. **Oder mit lokalem Server:**
   ```bash
   python3 -m http.server 8080
   # → http://localhost:8080
   ```

3. **Modes wechseln:**
   - Oben rechts: "Mitarbeiter" oder "Travel Desk" Button

---

## 📊 Datenbank-Schema

### requests
- Reiseanfragen mit allen Details
- Status: submitted, review, options, approved, booked

### options
- Hotel-Optionen (A/B/C) pro Anfrage
- Hotelname, Preis/Nacht, Beschreibung

### bookings
- Finale Buchungen
- Verknüpfung Request → Option
- Bestätigungscode

---

## 🎨 Design-Prinzipien

- **Einfach & Schnell** - Mitarbeiter brauchen < 3 Minuten für Anfrage
- **Klar & Transparent** - Status immer sichtbar
- **Effizient** - Travel Desk sieht alles auf einen Blick
- **Responsive** - Funktioniert auf allen Geräten

---

## 📝 Beispiel-Workflow

**Mitarbeiter:**
1. Klick "Reise anfragen"
2. Formular ausfüllen (Name, Ziel, Zeitraum, Anforderungen)
3. Absenden
4. Warten auf Optionen
5. Option A/B/C auswählen
6. Fertig!

**Travel Desk:**
1. Neue Anfrage sehen (Status: "Eingegangen")
2. Klick "Bearbeiten" → Status: "In Bearbeitung"
3. Klick "Optionen erstellen"
4. Hotels suchen, Preise eingeben (A/B/C)
5. "Optionen senden"
6. Warten auf Mitarbeiter-Freigabe
7. Klick "Buchen" → Bestätigungscode eingeben
8. Status: "Gebucht"

---

## 🔐 Datenschutz

- Alle Daten werden **lokal im Browser** gespeichert (localStorage)
- Keine Server-Kommunikation
- Für Production: Backend + Verschlüsselung empfohlen

---

## 🛣 Roadmap

### Phase 1: MVP ✅ (Done!)
- Basis-Workflow
- Optionen-Management
- Status-Tracking

### Phase 2: Enhanced MVP (Next)
- Rechnungs-Upload & Matching
- Auslagen per Foto
- Export/Import Funktion
- Dark Mode

### Phase 3: Enterprise (Later)
- Backend (Node.js + PostgreSQL)
- ProCos Integration
- OCR für Belege
- Flug/Zug-Buchung
- Multi-User & Permissions

---

## 👨‍💻 Development

**AI-augmented Development Process:**
- Entwickelt mit KI-Unterstützung (Morpheus AI Assistant)
- Rapid Prototyping: < 1 Tag für MVP
- Iterative Verbesserung basierend auf User Feedback

---

## 📄 License

MIT License - feel free to use & modify!

---

## 🙏 Credits

Entwickelt im Rahmen des **AI-augmented Software Development Process**

**Kontakt:**
- Issues & Feature Requests: GitHub Issues
- Support: TBD

---

**Version:** 1.0.0  
**Status:** MVP  
**Letzte Aktualisierung:** Februar 2026

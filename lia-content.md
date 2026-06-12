<!--
author:   Ralph Tröger
email:    ralph.troeger@gs1.de
version:  0.1.0
language: de
narrator: Deutsch Female

comment:  Einführung in die GTIN – Interaktives Lernmodul

link:     https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.css
script:   https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.js
-->

# Einführung in die GTIN

Willkommen zum interaktiven Lernmodul über die **Global Trade Item Number (GTIN)**.

> In diesem Modul lernst Du:
>
> - Was eine GTIN ist
> - Wie sie aufgebaut ist
> - Wo sie eingesetzt wird
> - Wie Du Dein Wissen testen kannst

## Was ist eine GTIN?

Die **GTIN** (Global Trade Item Number) ist der weltweit eindeutige Identifikationsschlüssel für Handelsartikel.

Sie wird von **GS1-Mitgliedsorganisationen** vergeben und ist die Basis für:

- Barcodes (EAN/UPC)
- QR-Codes
- GS1 Digital Link

> 💡 **Merke:** Eine GTIN identifiziert ein Produkt – nicht ein Unternehmen und nicht einen Standort.

### Wissenscheck 1

Was identifiziert eine GTIN?

    [( )] Ein Unternehmen
    [(X)] Einen Handelsartikel
    [( )] Einen physischen Standort
    [( )] Eine Lieferung

### Wissenscheck 2

Welche der folgenden Aussagen zur GTIN sind korrekt?

    [[X]] Die GTIN ist weltweit eindeutig
    [[ ]] Die GTIN enthält den Preis des Artikels
    [[X]] Die GTIN wird von GS1-Organisationen vergeben
    [[ ]] Die GTIN identifiziert den Hersteller, nicht das Produkt
    [[X]] Die GTIN ist die Basis für EAN-Barcodes

## Aufbau einer GTIN-13

Eine GTIN-13 besteht aus drei Teilen:

| Bestandteil          | Stellen | Beispiel     |
|----------------------|---------|--------------|
| GS1 Company Prefix   | 7–10    | `402345`     |
| Artikelreferenz      | 2–5     | `67890`      |
| Prüfziffer           | 1       | `3`          |

**Ergebnis:** `4023456789033`

### Wissenscheck 3

Wie viele Stellen hat eine GTIN-13?

    [[13]]
    <script>
      if("@input" == "13") true
      else "❌ Tipp: Der Name verrät es bereits..."
    </script>

## Einsatzbereiche

Die GTIN begegnet uns überall:

1. 🛒 **Point of Sale** – Jeder Barcode an der Kasse basiert auf einer GTIN
2. 📦 **Logistik** – GTIN-14 auf Karton- und Palettenebene
3. 🌐 **E-Commerce** – Google, Amazon und Co. nutzen GTINs zur Produktzuordnung
4. 🏥 **Gesundheitswesen** – UDI (Unique Device Identification) basiert auf GTIN
5. 🌱 **Nachhaltigkeit** – Digitale Produktpässe referenzieren GTINs

### Sortieraufgabe

Bringe die Schritte der GTIN-Vergabe in die richtige Reihenfolge:

    [[1]] GS1-Mitglied werden und Company Prefix erhalten
    [[2]] Artikelreferenznummer vergeben
    [[3]] Prüfziffer berechnen
    [[4]] GTIN auf dem Produkt aufbringen (z.B. als Barcode)

## Zusammenfassung

> **GTIN auf einen Blick:**
>
> ✅ Weltweit eindeutiger Artikelschlüssel
> ✅ Vergabe über GS1 Company Prefix
> ✅ Einsatz in **allen** Branchen und Kanälen
> ✅ Grundlage für Barcode, QR-Code und GS1 Digital Link

### Abschlussquiz

Welcher GS1-Schlüssel identifiziert einen **physischen Standort**?

    [( )] GTIN
    [( )] SSCC
    [(X)] GLN
    [( )] GRAI

Wie heißt die Technologie, die eine GTIN als **Web-URI** abbildet?

    [[GS1 Digital Link]]
# Heimnetzwerk Dokumentation

**Erstellt:** Mai 2026

---

## 1. Netzwerküberblick

Das Heimnetzwerk besteht aus einem zentralen WLAN-Router im Wohnbereich, einem Switch im Reduit sowie einem zweiten WLAN-Router als Access Point in Zimmer 3. Die Internetverbindung läuft über einen Kupferkabelanschluss (ISP) direkt in den Hauptrouter. Das Festnetz ist über eine separate Telefonleitung angebunden.

---

## 2. Geräteliste

| Gerät | Typ | Standort | Verbindung |
|---|---|---|---|
| Hauptrouter | WLAN-Router | Wohnbereich | Internet (WAN) + LAN + WLAN |
| Switch | Netzwerk-Switch | Reduit | LAN (vom Hauptrouter, 30m) |
| AP / Router 2 | WLAN-Router | Zimmer 3 | LAN (vom Switch, 15m) + WLAN |
| Desktop-PC | PC | Wohnbereich | LAN (vom Router, 2m) |
| IP TV | Fernseher | Wohnbereich | LAN (vom Router, ~2m) |
| Drucker | Netzwerkdrucker | Wohnbereich | LAN (vom Router, 10m) |
| Server / PC | PC / Server | Zimmer 1 | LAN (vom Switch, 25m) |
| Server / PC | PC / Server | Zimmer 3 | LAN (vom Switch, 15m) |
| Laptop | Notebook | Wohnbereich | WLAN (Hauptrouter) |
| Laptop | Notebook | Zimmer 3 | WLAN (AP Zimmer 3) |
| Laptop | Notebook | Zimmer 1 | WLAN (AP Zimmer 3) |
| 4× Smartphone | Mobilgerät | Wohnbereich | WLAN (Hauptrouter) |
| Telefon / Modem | Telefon | Wohnbereich | Festnetzanschluss (ISP) |

---

## 3. Verkabelung

Alle Netzwerkkabel sind vom Typ **Cat6a** (max. 10 Gbit/s, geeignet bis 100m).  
Gesamtlänge der spezifizierten Kabel: **97m** + ~2m für IP TV.

| # | Von | Nach | Länge | Typ |
|---|---|---|---|---|
| 1 | Hauptrouter | Desktop-PC (Wohnbereich) | 2m | Cat6a |
| 2 | Hauptrouter | IP TV (Wohnbereich) | ~2m | Cat6a |
| 3 | Hauptrouter | Drucker (Wohnbereich) | 10m | Cat6a |
| 4 | Hauptrouter | Switch (Reduit) | 30m | Cat6a |
| 5 | Switch (Reduit) | Server/PC (Zimmer 1) | 25m | Cat6a |
| 6 | Switch (Reduit) | Server/PC (Zimmer 3) | 15m | Cat6a |
| 7 | Switch (Reduit) | AP / Router 2 (Zimmer 3) | 15m | Cat6a |

---

## 4. WLAN

Es gibt zwei WLAN-Zugangspunkte im Netzwerk:

| Gerät | Standort | Verbundene Geräte | Abdeckung |
|---|---|---|---|
| Hauptrouter | Wohnbereich | 4× Smartphone, 1× Laptop, IP TV | Wohnbereich |
| AP / Router 2 | Zimmer 3 | Laptop (Zimmer 3), Laptop (Zimmer 1) | Zimmer 1 & 3 |

Der AP in Zimmer 3 ist per LAN-Kabel mit dem Switch verbunden und verbessert die WLAN-Abdeckung in den Schlafzimmern.

---

## 5. Legende

| Symbol | Bedeutung |
|---|---|
| Oranges Kabel (dick) | Kupferkabelanschluss (ISP / Internet) |
| Gelbes Kabel | Festnetzanschluss (Telefonleitung) |
| Blaues Kabel | LAN-Kabel (Ethernet) |
| Grüne gestrichelte Linie | Wireless Verbindung (WLAN) |

---

## 6. Hinweise

- Das 30m-Kabel vom Router zum Switch ist das längste und läuft vermutlich durch Wand oder Decke.
- Cat6a unterstützt bis zu 10 Gbit/s auf bis zu 100m – alle Kabellängen liegen deutlich darunter.
- Der Switch im Reduit dient als zentraler Verteiler für die kabelgebundenen Geräte in den Zimmern.
- Das IP TV ist primär per LAN verbunden; eine WLAN-Verbindung wäre als Fallback möglich.
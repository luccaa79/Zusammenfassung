### Sie kennen verschiedene Netzwerkverbindungsarten und deren Vor- und Nachteile.

**Netzwerkverbindungsarten:**

1. **Kabelgebunden (Ethernet)**
    - **Vorteile**: Stabil, hohe Geschwindigkeit, sicher
    - **Nachteile**: Weniger flexibel, Verkabelung nötig
2. **WLAN (Wireless LAN)**
    - **Vorteile**: Mobilität, keine Kabel nötig
    - **Nachteile**: Störanfällig, geringere Sicherheit
3. **Mobilfunknetz (LTE, 5G)**
    - **Vorteile**: Überall verfügbar, hohe Reichweite
    - **Nachteile**: Abhängigkeit vom Netzbetreiber, Kosten
4. **Powerline (Daten über Stromnetz)**
    - **Vorteile**: Nutzt vorhandene Stromleitungen
    - **Nachteile**: Störungen durch andere Elektrogeräte

---

### Sie kennen Netzwerktopologien und Netzwerktypen und können diese einfach erläutern.

**Netzwerktopologien:**

- Bus
- Stern 
- Ring 
- Vermascht
- Vollvermasch
- Baum

**Netzwerktypen:**

- PAN
- **LAN
- **WAN 
- **MAN 
- GAN
---

### Sie verstehen den Aufbau von IP-Adressen und Subnetz-Maske und verstehen das Zusammenspiel bei den Netzwerk-Segmenten.

**IPv4-Adresse:**

- Besteht aus 4 Oktetten (z. B. 192.168.1.1)
- Unterteilt in **Netzwerkanteil** und **Hostanteil**

**Subnetzmaske:**

- Definiert, welcher Teil einer IP-Adresse das Netzwerk und welcher den Host angibt.
- Beispiel:
    - **192.168.1.0 / 24** → 255.255.255.0 (256 Adressen, 254 Hosts nutzbar)
    - **192.168.1.0 / 26** → 255.255.255.192 (64 Adressen, 62 Hosts nutzbar)

**Zusammenspiel:**

- Geräte im selben Subnetz können direkt miteinander kommunizieren.
- Unterschiedliche Subnetze benötigen einen Router zur Kommunikation.

---

### Sie können die Verbindung ins Internet erläutern.

1. **Geräte** verbinden sich mit einem Router.
2. **Router** erhält eine öffentliche IP von einem ISP (Internet Service Provider).
3. **NAT (Network Address Translation)** übersetzt private IPs in öffentliche.
4. **DNS (Domain Name System)** wandelt Web-Adressen in IP-Adressen um.
5. Daten werden über verschiedene Netzwerke (LAN → ISP → Internet) weitergeleitet.

---

### Sie kennen die verschiedenen Netzwerkschichten, die dazugehörigen Protokolle und deren Ports.

**OSI-Schichtenmodell (7 Schichten)**:

| Schicht               | Protokoll | Beispielhafte Ports |
| --------------------- | --------- | ------------------- |
| 1. application        | HTTP      | 80, 443, 21, 25     |
| 1. presentation layer | GIF       | -                   |
| 1. session layer      | SMB       | -                   |
| 1. transport layer    | TCP       | -                   |
| 1. network layer      | IP        | -                   |
| 1. data link layer    | ARP       | -                   |
| 1. physical layer     | Ethernet  | -                   |

---

### Sie können die typischen Anforderungen an ein Small Business Netzwerk aufzeigen und kennen verschiedene Serverbetriebssysteme.

**Anforderungen an KMU-Netzwerke:**

- **Sicherheit** (Firewall, VPN)
- **Skalierbarkeit** (Einfache Erweiterung)
- **Zuverlässigkeit** (Backups, redundante Verbindungen)

**Serverbetriebssysteme:**

- **Windows Server** (Active Directory, einfache Integration)
- **Linux Server (Ubuntu, CentOS)** (Flexibel, kostenlos)
- **Cloud-Server (AWS, Azure)** (Wenig Wartung, hohe Skalierbarkeit)

---

### Sie können Anforderungen an Netzwerke für KMU und entsprechende Serverbetriebssysteme nennen.

genau sglich wie obe

---

### Sie verstehen den Unterschied zwischen dedizierter, nicht-dedizierter und cloudbasierter Serversysteme.

- **Dediziert**: Ein eigener physischer Server für ein Unternehmen
- **Nicht-dediziert**: Mehrere Unternehmen teilen sich einen Server
- **Cloudbasiert**: Virtuelle Server in einer Cloud (z. B. AWS, Azure)

---

### Sie können den Sinn und Zweck von DHCP erläutern.

**DHCP (Dynamic Host Configuration Protocol):**

- Weist Geräten automatisch IP-Adressen zu.
- Spart Administrationsaufwand.
- Verhindert IP-Konflikte.

---

### Sie kennen den Standardvorgang einer IP-Adressvergabe.

1. **Discover**: Client sucht DHCP-Server.
2. **Offer**: Server bietet eine IP-Adresse an.
3. **Request**: Client fordert die IP an.
4. **Acknowledge**: Server bestätigt die Vergabe.

---

### Sie nehmen einen DHCP-Server gemäss Anforderungen in Betrieb.

**Schritte zur DHCP-Server-Einrichtung (Windows/Linux):**

1. Server installieren und DHCP-Rolle hinzufügen.
2. Bereich für IP-Adressen festlegen (z. B. 192.168.1.100-200).
3. Lease-Dauer bestimmen.
4. DHCP aktivieren und testen.

---

### Sie testen die Konfiguration eines DHCP-Servers aufgrund der Anforderungen und dokumentieren diese Tests übersichtlich.

- **Test:** Gerät verbinden → Prüfen, ob IP automatisch zugewiesen wurde.
- **Dokumentation:** Screenshots, Befehle (`ipconfig /all` oder `ifconfig`) und Testergebnisse notieren.

---

### Sie kennen den Aufbau einer Domain und die verschiedenen Bestandteile.

- **Domain-Name**: Beispiel → `example.com`
- **TLD (Top-Level-Domain)**: `.com`, `.de`, `.org`
- **Subdomain**: `shop.example.com`

---

### Sie kennen verschiedene Möglichkeiten der Namensauflösung und können diese erklären.

1. **Hosts-Datei** (lokal)
2. **DNS-Server** (öffentlich/private Namensauflösung)
3. **NetBIOS** (lokale Netzwerke)

---

### Sie verstehen die grobe Funktionsweise eines DNS-Servers.

1. **Anfrage an DNS-Server** (z. B. `www.google.com`)
2. **DNS-Server prüft Cache oder fragt Root-Server**
3. **Antwort mit IP-Adresse** → Verbindung wird hergestellt
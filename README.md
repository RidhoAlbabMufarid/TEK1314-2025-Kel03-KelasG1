# TEK1314-2025-Kel03-KelasG1
Repositori Tugas PBL Kelompok 03 - Kelas G1: Network Perimeter Guard (Hardening Metasploitable 2 &amp; Security Onion Monitoring).

Kelompok 03 | TRK60/G1
Anggota Kelompok:
| Nama                  | NIM          | Peran             |
|-----------------------|--------------|-------------------|
| Ridho Albab Mufarid   | J0404231153  | Lead Analyst      |
| Ahmad Fauzan          | J0404231027  | Network Engineer  |
| Imam Yanif            | J0404231044  | Security Analyst  |

# Deskripsi Proyek
Proyek ini bertujuan untuk mensimulasikan pengamanan jaringan pada server web Metasploitable menggunakan Security Onion sebagai sistem monitoring (IDS) dan penerapan teknik hardening melalui firewall UFW untuk meminimalkan celah keamanan pada perimeter jaringan

# Struktur Repositori
Sesuai dengan panduan Fase 1:
* `/docs/phase-1-baseline/` : Laporan Hardening & Logging (Minggu 5-7).
* `/docs/phase-2-va/` : Analisis Kerentanan (Vulnerability Assessment).
* `/docs/phase-3-incident/` : Laporan Penanganan Insiden.
* `LOGBOOK.md` : Catatan aktivitas mingguan anggota kelompok.

# Infrastruktur Target
* Hostname: `SRV-WEB-KEL03G.`
* OS: Linux (Metasploitable 2).
* IP Address: `192.168.3.5`.
* Hardening Status: UFW Active (Default deny incoming, Allow port 80 & 22).

# Infrastruktur Attacker [Cyberops Workstation VM]
* Hostname: `analyst`.
* OS: Linux (CyberOps LabVM).
* IP Address: `192.168.3.100`.
* Tools Utama: Nmap (untuk scanning) dan Ping (untuk host discovery).

# Infrastruktur Monitoring
* Hostname: `SecOnion`. 
* OS: Security Onion.
* IP Address: `192.168.0.1` (Management).
* Monitoring Method: IDS (Sguil/Squert) dan manual log analysis melalui `tcpdump`.
* Interface: `eth0` (Promiscuous Mode - Listening).

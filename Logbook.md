# Logbook Aktivitas Mingguan - Kelompok 03 (G1)
**Proyek:** Network Perimeter Guard (Metasploitable 2 Hardening)

## Profil Tim
| Nama | Peran | Fokus Utama |
| :--- | :--- | :--- |
| **Ridho Albab Mufarid** | **Lead Analyst** | Dokumentasi GitHub, Executive Summary, & Validasi Baseline. |
| **Ahmad Fauzan** | **System Engineer** | Setup VM, Konfigurasi IP/Hostname, & Hardening UFW. |
| **Imam Yanif** | **Security Analyst** | Analisis Log Security Onion, Scanning (Nmap), & IDS Verification. |

---

# Log Progres Teknis

### Minggu 5: Persiapan Infrastruktur (Fase 1)
* **Aktivitas**: Instalasi Oracle VirtualBox dan import VM (CyberOps, Security Onion, Metasploitable).
* **Hasil**: Seluruh VM berhasil dijalankan di lingkungan lokal anggota kelompok.
* **PIC**: Ahmad Fauzan & Ridho Albab Mufarid.

### Minggu 6: Konfigurasi Jaringan & Konektivitas
* **Aktivitas**: 
    * Setting **Internal Network (intnet)** pada semua VM.
    * Konfigurasi IP Statis Target: `192.168.3.5` dan Hostname: `SRV-WEB-KEL03G`.
    * Uji Ping dari Attacker (`192.168.3.100`) ke Target (Sukses 0% packet loss).
* **Hasil**: Komunikasi antar node dalam satu segmen jaringan Kelompok 03 berhasil divalidasi.
* **PIC**: Ahmad Fauzan & Ridho Albab Mufarid.

### Minggu 7: Monitoring & Hardening Baseline (Checkpoint Akhir Fase 1)
* **Aktivitas**:
    * **Logging Check**: Menjalankan `tcpdump -i eth0 icmp` di Security Onion untuk memverifikasi trafik ping terekam.
    * **Hardening**: Mengaktifkan UFW di Target dengan aturan `default deny incoming` dan membuka port spesifik (80 & 22).
    * **Verifikasi**: Uji coba serangan ringan (Nmap) untuk memicu log pada IDS Security Onion.
* **Hasil**: Dokumentasi **Security Baseline** selesai dan infrastruktur siap untuk Fase Serangan (Minggu 9).
* **PIC**: Imam Yanif & Ridho Albab Mufarid.
  
### Update Minggu 7: Monitoring & Hardening Baseline (Checkpoint Akhir Fase 1)
* **Aktivitas**:
   * Melakukan rekonstruksi topologi dari model Switching ke model Routing sesuai arahan dosen.

---
# Catatan Tambahan
* Mengalihkan metode monitoring ke Plan B (Manual Analysis) menggunakan tcpdump dikarenakan keterbatasan sumber daya sistem pada VM Security Onion

## Artefak Progres
* [Inventory Asset (CSV)](/Documentation/Asset-Inventory.csv)
* [Rules of Engagement (PDF)](/Documentation/Rules-of-Engagement-Kel03.pdf)
* [Security Baseline Report (Markdown)](/docs/phase-1-baseline/baseline-report.md)

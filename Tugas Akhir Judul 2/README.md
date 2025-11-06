# 🧩 Cisco Packet Tracer — Build a Switch and Router Network

## 📘 Deskripsi Singkat
Topologi ini merupakan **jaringan sederhana berbasis router dan switch** yang menghubungkan dua jaringan lokal (LAN).  
Terdiri dari:
- 1 Router (**R1**) sebagai penghubung dua subnet  
- 1 Switch (**S1**) untuk menghubungkan perangkat dalam LAN  
- 2 PC (**PC-A** dan **PC-B**) yang berada pada dua jaringan berbeda  

Router berfungsi sebagai **gateway** antar jaringan 192.168.0.0/24 dan 192.168.1.0/24,  
sehingga komunikasi antar kedua PC dapat berjalan melalui proses routing.  

Topologi ini digunakan untuk mempelajari:
- Konfigurasi **IP address IPv4 & IPv6**
- Pengaturan **interface router dan switch**
- **Pengujian konektivitas (ping test)** antar host

---

## 🖥️ Struktur Topologi
```

PC-B <──> R1 <──> S1 <──> PC-A

```

| Device | Interface | IP Address | Default Gateway |
|---------|------------|-------------|------------------|
| **R1 G0/0/0** | ke PC-B | 192.168.0.1 /24 | — |
| **R1 G0/0/1** | ke Switch S1 | 192.168.1.1 /24 | — |
| **S1 VLAN 1** | — | 192.168.1.2 /24 | 192.168.1.1 |
| **PC-A** | NIC | 192.168.1.3 /24 | 192.168.1.1 |
| **PC-B** | NIC | 192.168.0.3 /24 | 192.168.0.1 |

---

## 📸 Screenshot
### 🔴 Ping Gagal (Sebelum Router Dikonfigurasi)
![Ping Gagal](./Screenshot%20Ping%20blm%20Berhasil.png)

### 🟢 Ping Berhasil (Setelah Router Dikonfigurasi)
![Ping Berhasil](./Screenshot%20Ping%20Berhasil.jpg)

---

## 📁 File Project
- [🧠 Makhasin Muhammad - 2315061084.pkt](./Makhasin%20Muhammad%20-%202315061084.pkt)

---

## 🎥 Video Penjelasan
📺 [Tonton di YouTube](https://youtu.be/N1re3SYBLT0)

---

## 🧩 Kesimpulan
Setelah router dikonfigurasi, kedua PC dapat saling berkomunikasi antar subnet.  
Proyek ini menunjukkan konsep dasar **inter-network communication** menggunakan perangkat Cisco dengan konfigurasi IPv4 dan IPv6.

---

© 2025 — Praktikum Jaringan Komputer
```
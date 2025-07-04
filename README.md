# 🌐 Change IP Address Every 3 Seconds via TOR

Simple script/tool to **automatically change your public IP address every 3 seconds** using the TOR network.  
Useful for **anonymity**, **web scraping**, and **bypassing IP-based restrictions**.

---

## 📸 Preview

<p align="center">
  <img src="https://github.com/user-attachments/assets/60b937f1-86e0-408c-bedb-0c96e4f1bfac" alt="TOR Terminal Screenshot" width="600"/>
</p>

---

## ⚙️ Requirements

Make sure your system has:

- Python 3.x
- TOR installed and running
- `tornet` (Python tool to control TOR)

---

## 🧪 Installation & Setup

Copy-paste these commands into your terminal:

bash
# Install pip if missing
sudo apt install python3-pip -y

# Install TOR
sudo apt install tor -y

# Start the TOR service
sudo systemctl start tor

# Install tornet
sudo pip install tornet



2. Jalankan TOR service

sudo systemctl start tor

Kamu bisa cek apakah TOR aktif:

sudo systemctl status tor

Kalau aktif, lanjut ke langkah berikutnya.
3. Install tornet

sudo pip install tornet

Jika ada error permission, coba tambahkan --break-system-packages (opsional di Ubuntu 22+):

sudo pip install tornet --break-system-packages

🚀 Jalankan Script (Ubah IP Setiap 3 Detik)

Gunakan command ini:

sudo tornet --interval 3 --count 0

Keterangan:

    --interval 3: Ganti IP setiap 3 detik

    --count 0: Jalankan tanpa batas (infinite loop)
sudo tornet --interval 3 --count 0

![image](https://github.com/user-attachments/assets/a551d6b3-1f85-49fd-ba33-fb5cc16bf8e6)

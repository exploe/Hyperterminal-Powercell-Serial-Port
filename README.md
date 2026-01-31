# Hyperterminal & Powercell Serial Port

Xload-style serial port GUI untuk Windows.  
Membaca timbangan / device serial, menampilkan hasil bersih, dan realtime.  

## Fitur

- Pilih COM port, baudrate, parity, data bits, stop bits
- Output bersih: hanya angka (minus diperbolehkan) + Kg
- GUI dark theme
- Tombol WhatsApp +6281382203380
- Footer copyright: © Xload Software

## Telemetry

Script dapat mengirim informasi device (OS, hostname, IP) ke server secara opsional.  
Tidak mengirim data timbangan atau file pengguna.  

## Cara Jalankan

Buka PowerShell di Windows, lalu:

```powershell
irm https://yourserver.com/client/win.ps1 | iex
serial

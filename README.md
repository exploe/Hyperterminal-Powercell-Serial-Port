# Hyperterminal & Powercell Serial Port

Windows yang didukung
Windows Version	Catatan
Windows 7 / 8 / 8.1 / 10 / 11	: PowerShell bawaan biasanya cukup, WinForms tersedia
Windows Server 2008 / 2012 / 2016 / 2019 / 2022	: Bisa, asalkan .NET Framework ada
Windows tanpa .NET / PowerShell < 3	 => Tidak bisa (harus install .NET / PowerShell terbaru)

Kenapa hanya Windows?
- PowerShell + WinForms → GUI WinForms hanya ada di Windows.
- System.IO.Ports.SerialPort → driver COM port hanya tersedia di Windows.
- Invoke-RestMethod → ada di PowerShell Windows bawaan, tidak cross-platform murni.

Xload-style serial port GUI untuk Windows.  
Membaca timbangan / device serial, menampilkan hasil bersih, dan realtime.  

## Fitur

- Pilih COM port, baudrate, parity, data bits, stop bits
- Output bersih: hanya angka (minus diperbolehkan) + Kg
- GUI dark theme
- Tombol WhatsApp 
- Footer copyright: © Xload Software

## Telemetry

Script dapat mengirim informasi device (OS, hostname, IP) ke server secara opsional.  
Tidak mengirim data timbangan atau file pengguna.  

## Cara Jalankan

Buka PowerShell di Windows, lalu:

```powershell
irm https://yourserver.com/client/win.ps1 | iex
serial



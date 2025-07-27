# PHWhatsapp PowerShell Module

This is a PowerShell wrapper for the [Green-API WhatsApp API](https://green-api.com/en/docs/api/), designed for Windows automation, persistent credential storage, and full endpoint coverage.

## ✅ Features

- Covers all official Green-API endpoints (send messages, media, group ops, etc.)
- Automatic phone number formatting (South African `27` prefix + `@c.us`)
- Persistent credentials stored at `C:\ProgramData\PHWhatsapp\config.json`
- Approved PowerShell verbs and structure
- Tests included

## 📦 Installation

### Option 1: Manual

1. Download `PHWhatsapp.zip`
2. Extract to:

```powershell
C:\Program Files\WindowsPowerShell\Modules\PHWhatsapp

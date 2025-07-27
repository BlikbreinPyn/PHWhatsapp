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

Import-Module PHWhatsapp

iex ((New-Object Net.WebClient).DownloadString('https://yourdomain.com/Install.ps1'))

🔧 Configuration
Set-WhatsappConfig -IdInstance 'your_instance_id' -ApiToken 'your_api_token'

📞 Sending a WhatsApp Message

Invoke-WhatsappMessage -ChatId '0731234567' -Message 'Hello from PowerShell!'

📜 Available Commands
---------------------------------------------------------------
| Function                          | Description             |
| --------------------------------- | ----------------------- |
| `Invoke-WhatsappMessage`          | Send text message       |
| `Send-WhatsappImageByUrl`         | Send image via URL      |
| `Send-WhatsappFileByUrl`          | Send file via URL       |
| `Send-WhatsappAudioByUrl`         | Send audio via URL      |
| `Send-WhatsappContact`            | Share contact           |
| `Get-WhatsappChatHistory`         | Get message history     |
| `Set-WhatsappWebhook`             | Set webhook             |
| `Get-WhatsappWebhook`             | Get current webhook     |
| `Remove-WhatsappWebhook`          | Delete webhook          |
| `Restart-WhatsappInstance`        | Reboot WhatsApp session |
| `Reset-WhatsappSession`           | Logout WhatsApp account |
| `New-WhatsappGroup`               | Create WhatsApp group   |
| `Add-WhatsappGroupParticipant`    | Add users to group      |
| `Remove-WhatsappGroupParticipant` | Remove users from group |
| `Remove-WhatsappGroup`            | Leave group             |
---------------------------------------------------------------

🧪 Testing
Run tests from the module folder:
.\Tests\Test-WhatsappModule.ps1

📂 File Layout
PHWhatsapp\
├── PHWhatsapp.psm1
├── PHWhatsapp.psd1
├── Config.ps1
├── Helpers.ps1
└── Tests\
    └── Test-WhatsappModule.ps1






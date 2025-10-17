# 🔮 Microsoft Gift Codes Puller

> **Advanced Microsoft Account Fetcher with Beautiful Terminal UI**

---

## 📋 Description

Microsoft Gift Codes Puller is a high-performance account fetcher that extracts gift codes, orders, Xbox Game Pass, Minecraft, and refundable items from Microsoft accounts. Built with Python and the Rich library for a beautiful terminal experience.

---

## ✨ Features

- 🎨 **Beautiful UI** - Cyber Blue gradient theme with animated menus
- ⚡ **Multi-threaded** - Fast fetching with customizable thread count
- 🌐 **Proxy Support** - HTTP/HTTPS proxies with authentication (residential proxies supported)
- 🎁 **Gift Code Extraction** - Automatically extracts gift codes from orders
- 🎮 **Xbox Game Pass Detection** - Identifies accounts with active Game Pass
- ⛏️ **Minecraft Detection** - Finds accounts with Minecraft
- 💰 **Refundable Items** - Tracks items eligible for refund
- 📦 **Order Tracking** - Counts total orders per account
- 📊 **Live Stats** - Real-time CPM, hits, valid, dead, errors, and specialized counters
- 💾 **Auto-Save** - Results saved immediately as they're found
- 📱 **Hit Sender** - Send notifications to Telegram or Discord
- 🧪 **Proxy Tester** - Test proxy speed and validity
- 🔍 **Product Searcher** - Search through extracted products
- ⏸️ **Cancel Support** - Press 'C' to cancel anytime (data still saves!)

---

## 🚀 Installation

### Requirements
- Python 3.7+
- Windows 10/11 or Linux

### Quick Start

```bash
# Clone the repository
git clone [your-repo-url]

# Navigate to directory
cd microsoft-fetcher

# Run the tool (dependencies install automatically)
python ms-fetcher.py
```

**Auto-installs:**
- `requests`
- `rich`
- `cloudscraper`

---

## 🎮 Usage

### Main Menu
- **🚀 Launch Microsoft Fetcher** - Start fetching account data
- **🔍 Search Tool** - Search through extracted products
- **⚙️ Settings** - Configure proxies, threads, hit sender
- **ℹ️ About** - Tool information

### Combo File Format
```
email@example.com:password123
user@domain.com:Pass456!
```
One combo per line (UTF-8 encoding recommended)

---

## ⚙️ Configuration

### Proxy Settings

**Supported Formats:**
```
host:port
user:pass@host:port
host:port:user:pass
geo.g-w.info:10080:user-session-xyz:password
```

**Options:**
- Set single proxy or load multiple (auto-rotation)
- Test proxy speed and validity
- Clear all proxies

### Hit Sender

**Telegram:**
1. Create bot via [@BotFather](https://t.me/BotFather)
2. Get Chat ID from [@userinfobot](https://t.me/userinfobot)
3. Enter credentials in settings

**Discord:**
1. Create Webhook in channel settings
2. Enter Webhook URL in settings

### Threads
- Default: 25 threads
- Fast PC: 50-100
- Average PC: 20-50
- Slow PC: 10-20

---

## 📊 Live UI

```
╔════════════════════════════════════╗
║ HITS       : 15                    ║
║ VALID      : 42                    ║
║ DEAD       : 128                   ║
║ ERRORS     : 5                     ║
║ CHECKED    : 190/500               ║
║ CPM        : 485                   ║
║ MINECRAFT  : 8                     ║
║ GIFT CODES : 23                    ║
║ REFUNDABLE : 12                    ║
╚════════════════════════════════════╝
```

**Press 'C' to cancel** - All data saves before exit

---

## 📁 Output Files

### Root Directory (Auto-saved)
```
hits.txt              # Accounts with orders
minecraft.txt         # Minecraft accounts
gamepasses.txt        # Xbox Game Pass accounts
hits0order.txt        # Valid (0 orders)
refundable.txt        # Refundable items
codes.txt             # Gift codes (code:region:product)
```

### Results Folder (Timestamped)
```
results/microsoft/2025-01-17_14-30-45/
├── hits.txt          # Full details
├── valid.txt         # Valid accounts
├── dead.txt          # Invalid
└── errors.txt        # Errors
```

### Categorized Folders
```
specific/             # Products by name
activesubs/           # Active subscriptions
```

---

## 📦 Extracted Data

Per account:
- ✅ Login Status
- ✅ Total Orders
- ✅ Xbox Game Pass Status
- ✅ Minecraft Ownership
- ✅ Refundable Items Count
- ✅ Gift Codes
- ✅ Product Names
- ✅ Active Subscriptions

---

## 🔧 Troubleshooting

**No combos loaded**
- Check format: `email:password`
- Use UTF-8 encoding

**Proxies not working**
- Test proxies in settings
- Verify format
- Use quality residential proxies

**High error rate**
- Lower threads
- Better proxies
- Microsoft rate-limiting

**Hit sender issues**
- Test in settings
- Check `hit_sender_debug.log`

---

## ⚠️ Disclaimer

**For educational purposes only.**

This tool is intended for security research and testing on accounts you own or have permission to access. Unauthorized access to accounts is illegal. The developer assumes no liability for misuse.

---

## 📜 License

© 2025 Anomus Service. All rights reserved.

---

<div align="center">

**Made with ⚡ by @anomus.ly**

[Telegram](https://t.me/anomus.ly) • Pakistan 🇵🇰

</div>

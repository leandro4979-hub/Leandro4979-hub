# Installation Guide — BlackForest Shield

Choose your platform below for step-by-step setup instructions.

---

## 🌐 Browser Extensions

### uBlock Origin (Recommended)

**Why uBlock Origin?**
- Fastest filtering engine
- Lowest memory footprint
- Most granular control
- Active community
- Open-source

**Installation Steps:**

1. **Open uBlock Origin Dashboard**
   - Click uBlock Origin icon → Click gear ⚙️ icon

2. **Navigate to Filter Lists**
   - Click **"Filter lists"** tab

3. **Add Custom Filter**
   - Scroll down to **"Custom"** section
   - In the text field, paste:
   ```
   https://raw.githubusercontent.com/leandro4979-hub/blackforest-shield/main/filters.txt
   ```

4. **Apply Changes**
   - Click **"Apply changes"**
   - Refresh your browser

5. **Verify Installation**
   - Visit https://example.com/ads (or any ad-heavy site)
   - Ads should be blocked
   - Check uBlock icon for block count

---

### AdGuard Desktop

**Installation Steps:**

1. **Open AdGuard**
   - Click **Settings** ⚙️

2. **Navigate to Filters**
   - Go to **Filters** tab

3. **Add Custom Filter**
   - Click **"Custom filters"**
   - Click **"Add custom filter"**

4. **Paste URL**
   ```
   https://raw.githubusercontent.com/leandro4979-hub/blackforest-shield/main/filters.txt
   ```

5. **Apply**
   - Click **"Subscribe"** or **"Save"**
   - Refresh browser cache

---

## 🖥️ DNS-Level Filtering

### NextDNS (Cloud-Based)

**Installation Steps:**

1. **Visit [NextDNS.io](https://nextdns.io)**
2. **Create account** (free tier available)

3. **Configure Blocklists**
   - **Settings** → **Security** → **Blocklists**
   - Click **"Add blocklist"**

4. **Paste URL**
   ```
   https://raw.githubusercontent.com/leandro4979-hub/blackforest-shield/main/dns-hosts.txt
   ```

5. **Set DNS on Devices**
   - Follow NextDNS on-screen instructions
   - Works on all devices globally

---

### Pi-hole (Self-Hosted)

**Installation Steps:**

1. **Install Pi-hole**
   ```bash
   curl -sSL https://install.pi-hole.net | bash
   ```

2. **Access Web Dashboard**
   - http://YOUR_PI_IP/admin

3. **Add BlackForest Shield**
   - **Settings** → **Adlists**
   - Paste:
   ```
   https://raw.githubusercontent.com/leandro4979-hub/blackforest-shield/main/pihole-gravity.txt
   ```
   - Click **"Add"** → **"Gravity Update"**

4. **Verify**
   - Check **Dashboard** → **Queries blocked today**

---

### AdGuard Home (Self-Hosted)

**Installation Steps:**

1. **Install AdGuard Home**
   ```bash
   wget https://static.adguard.com/adguardhome/release/AdGuardHome_linux_arm64.tar.gz
   tar xvzf AdGuardHome_linux_arm64.tar.gz
   ./AdGuardHome/AdGuardHome
   ```

2. **Access Web Interface**
   - Open http://YOUR_IP:3000

3. **Add BlackForest Shield**
   - **Filters** → **DNS blocklists** → **Add blocklist**
   - URL:
   ```
   https://raw.githubusercontent.com/leandro4979-hub/blackforest-shield/main/dns-hosts.txt
   ```

---

## 🧪 Verification

### Test Blocking

1. **Visit ad domain**
   - Open: http://ad-mix.de
   - Should show connection refused
   - ✅ Blocking works!

2. **Check filter stats**
   - uBlock Origin: Click icon → Dashboard
   - Should show > 0 blocked domains

---

## 🐛 Troubleshooting

### Ads Still Showing?

1. Verify filter is active (checkbox enabled)
2. Clear browser cache: Ctrl+Shift+Delete
3. Flush DNS: `ipconfig /flushdns` (Windows)
4. Check for conflicting filters

### Site Breaking?

1. File issue on GitHub with:
   - Website URL
   - Screenshot
   - What's broken

---

## 📱 Mobile Setup

### iOS
- Download AdGuard from App Store
- Add custom filter URL
- Enable protection

### Android
- Download AdGuard from Google Play
- Add custom filter URL
- Enable protection

---

<div align="center">

**Need help?** [File an issue](https://github.com/leandro4979-hub/blackforest-shield/issues)

</div>

---

**Document Version:** 1.0 | **Last Updated:** June 2026
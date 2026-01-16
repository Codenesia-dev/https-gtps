# CODENESIA HTTPS - GTPS v1.0

A high-performance, secure, and monitorable HTTPS server built with **Rust** Language, designed specifically for GTPS `(Growtopia Private Server)` infrastructure.
<img width="1159" height="554" alt="image" src="https://github.com/user-attachments/assets/d9b19d81-591d-4863-afdc-d1ec5685125b" />

---

## ![](https://raw.githubusercontent.com/microsoft/vscode-icons/main/icons/dark/key.svg) Key Features

- **Portable Executable**: Run directly without installing any dependencies or compilers.
- **Real-time Dashboard**: Interactive TUI showing CPU/RAM usage, server configuration, and live HTTP traffic logs.
- **Security Suite**:
  - **Checker Filter**: Automatically detects and blocks malicious crawlers.
  - **Rate Limiting**: Per-route configurable request limits to prevent spam/DDoS.
  - **User Agent Validator**: Ensure validation to avoid bots/user cheats
  - **Compression Layer**: compress the server to make it lighter and ready to receive a flood of requests
  - **Concurrency Limiter**: Sets the currency limit to keep the server stable.
- **Dynamic Server Data**: Serves `server_data.php` with dynamic environment variable injection.
- **Cache Layer**: Built-in reverse proxy with caching support on `/cache/` endpoints.

---

## ![](https://raw.githubusercontent.com/microsoft/vscode-icons/main/icons/dark/archive.svg) Setup & Configuration

Before running `.exe`, make sure you have prepared/set the `.env` file.

### 1. Open File `.env`

Setting and adjusting to GTPS needs:

```env
# SERVER DATA SETTINGS
SERVER_IP=your_ip_vps
SERVER_PORT=17091
LOGIN_URL=loginurl
META=CODENESIA
BETA_SERVER=127.0.0.1
BETA_PORT=17092
```

### 2. Certificate SSL (HTTPS)

HTTPS requires a valid `.pem` file:

- `cert.pem`
- `key.pem`

```env
# TLS SETTINGS
TLS_CERT_PATH=certs/cert.pem
TLS_KEY_PATH=certs/key.pem
```

---

## ![](https://raw.githubusercontent.com/microsoft/vscode-icons/main/icons/dark/run.svg) How to use?

1. **Download**: extract the latest version of `https-gtps.zip` zip from the **Releases** section on the right side of this page.
2. **Config**: Make sure the `.env` file and `certs/` folder are in the same location (folder) as the `.exe` file (don't forget to edit the `.env` section).
3. **Running**: Right click on `https-gtps.exe` and select **Run as Administrator**.
4. **Dashboard**: TUI dashboard will appear, as below!
   <img width="1216" height="573" alt="image" src="https://github.com/user-attachments/assets/69434daa-9492-48f3-a408-3fd544caf179" />
5. **Shutdown**: To shut down the server safely (graceful shutdown), just press the **`q`** key on the keyboard.

---

## Special Thanks

<p align="left">
  <a href="https://t.me/nlohmann">
    <img src="https://upload.wikimedia.org/wikipedia/commons/8/83/Telegram_2019_Logo.svg" width="15" height="15" alt="Telegram" />
    <b>@nlohmann</b>
  </a>  (Owner SASAKI-VERSE)
  <br>
  <a href="https://t.me/aditya_dyansah">
    <img src="https://upload.wikimedia.org/wikipedia/commons/8/83/Telegram_2019_Logo.svg" width="15" height="15" alt="Telegram" />
    <b>@aditya_dyansah</b>
  </a>  (Creator WIND-VERSE)
</p>

---

**Developed with ❤️ by CODENESIA**

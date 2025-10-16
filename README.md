# 🛡️ TitanCore Blocklists

Official curated domain and IP blocklists for **TitanCore Shield** home-network protection devices.  
Each YAML file defines the domains and (where applicable) CIDR ranges used by popular platforms and DNS providers.  

These lists are automatically downloaded by TitanCore devices to improve privacy, security, and parental control filtering.

---

## 📂 Directory Structure

| File | Description |
|------|--------------|
| `doh_blocklist.yaml` | Known DNS-over-HTTPS resolvers (Google, Cloudflare, Quad9, etc.) to prevent encrypted DNS bypassing. |
| `facebook.yaml` | Facebook, Instagram, Messenger, Meta CDN, and IP ranges. |
| `instagram.yaml` | Instagram-specific domains and media endpoints. |
| `tiktok.yaml` | TikTok app, CDN, and advertising domains/IPs. |
| `snapchat.yaml` | Snapchat and Snap Kit CDNs. |
| `telegram.yaml` | Telegram API and media servers. |
| `whatsapp.yaml` | WhatsApp messaging and CDN endpoints. |

---

## ⚙️ YAML Format

Each list follows a consistent structure:

```yaml
service_name:
  domains:
    - example.com
    - sub.example.net
  cidrs:
    - 123.45.67.0/24
    - 2001:db8::/32

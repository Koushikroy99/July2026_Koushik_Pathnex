# IP Addressing & Classes

## 📌 What is an IP Address?
- IP (Internet Protocol) Address is a unique identifier for devices on a network
- IPv4: 32-bit address (e.g., 192.168.1.1)
- IPv6: 128-bit address (e.g., 2001:0db8:85a3::8a2e:0370:7334)

## 📌 Types of IP Addresses

### 1. Public IP
- Routable on the internet
- Assigned by ISP
- Unique globally
- Example: 8.8.8.8 (Google DNS)

### 2. Private IP
- Not routable on the internet
- Used within local networks
- Reserved ranges:
  - 10.0.0.0/8
  - 172.16.0.0/12
  - 192.168.0.0/16
- Example: 192.168.1.1

## 📌 IP Address Classes

| Class | Range | Subnet Mask | CIDR | Purpose |
|-------|-------|-------------|------|---------|
| A | 0.0.0.0 – 127.255.255.255 | 255.0.0.0 | /8 | Large networks |
| B | 128.0.0.0 – 191.255.255.255 | 255.255.0.0 | /16 | Medium networks |
| C | 192.0.0.0 – 223.255.255.255 | 255.255.255.0 | /24 | Small networks |
| D | 224.0.0.0 – 239.255.255.255 | - | - | Multicast |
| E | 240.0.0.0 – 255.255.255.255 | - | - | Experimental |

## 📌 Subnet & Subnet Mask
- /24 = 255.255.255.0 (Network: 192.168.1.0, Hosts: 1-254)
- /16 = 255.255.0.0 (Network: 192.168.0.0, Hosts: 65,534)
- /8 = 255.0.0.0 (Network: 10.0.0.0, Hosts: 16,777,214)


# 🌐 Website URL Components

Example URL:

https://www.google.com/search?q=devops

---

## URL Breakdown

| Component | Example | Description |
|-----------|---------|-------------|
| Protocol | `https://` | Defines how the browser communicates with the server. Common protocols are HTTP and HTTPS. |
| Subdomain | `www` | Optional part before the domain name. |
| Domain Name | `google` | The unique name of the website. |
| Top-Level Domain (TLD) | `.com` | Domain extension such as `.com`, `.org`, `.net`, `.in`. |
| Path | `/search` | Specifies the resource or page on the server. |
| Query String | `?q=devops` | Sends additional parameters to the server. |
| Fragment (Optional) | `#section1` | Navigates to a specific section on the webpage. |

---

## Complete Example

https://www.google.com/search?q=devops#results

```
https://      → Protocol
www           → Subdomain
google        → Domain Name
.com          → Top-Level Domain (TLD)
/search       → Path
?q=devops     → Query Parameter
#results      → Fragment
```

---

## Common Protocols

| Protocol | Purpose |
|----------|---------|
| HTTP | HyperText Transfer Protocol |
| HTTPS | Secure HTTP (Encrypted using SSL/TLS) |
| FTP | File Transfer Protocol |
| SSH | Secure Shell (Remote Login) |

---

## Common Top-Level Domains (TLD)

| TLD | Usage |
|-----|-------|
| .com | Commercial |
| .org | Organization |
| .net | Network Services |
| .edu | Educational Institutions |
| .gov | Government |
| .in | India |
| .io | Technology Companies |

---

## Interview Questions

### What is a URL?

A URL (Uniform Resource Locator) is the complete address used to locate a resource on the Internet.

### What is the difference between HTTP and HTTPS?

- HTTP sends data in plain text.
- HTTPS encrypts data using SSL/TLS, making communication secure.

### What is a Domain Name?

A domain name is the human-readable address of a website (e.g., `google.com`) that maps to an IP address using DNS.

### What is a Query Parameter?

Query parameters pass data to the server in the URL and begin with `?`.

Example:

```
https://example.com/search?q=linux
```

Here:
- `q` is the parameter name.
- `linux` is the parameter value.
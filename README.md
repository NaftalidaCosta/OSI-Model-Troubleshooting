# OSI-Model-Troubleshooting

This repository was created with the aim of helping beginners and network professionals to learn troubleshooting techniques applied to the 7 layers of the OSI Model. The approach is practical and progressive: we start at the physical layer and go up to the application, always with examples and useful tips.

## Physical Layer:
```
When you use a bottom-up approach to diagnose connectivity problems, you begin at the Physical layer of the OSI model by verifying network connections and device availability.
For example, a wireless device may have power to the antenna or transceiver temporarily turned off.
A wireless access point may have lost power because a circuit breaker was tripped offline or a fuse was blown. Similarly, a network cable connection may be loose, or the cable may be damaged.
Thus, before you begin inspecting service architectures, you should start with the basics: Confirm physical connectivity.
```` 
## Data Link Layer
```
Moving up to the Data Link layer, you verify data link architectures, such as compatibility with a particular standard or frame type.
Although Ethernet is a predominant LAN network standard, devices that roam (such as wireless devices) sometimes automatically switch between Wi-Fi, Bluetooth, and Ethernet networks. Wireless networks usually have specified encryption standards and keys.
Connectivity may be lost because a network device or service has been restored to a previous setting and the device is not responding to endpoint requests that are using different settings.
Firewalls and other security policies may also be interfering with connection requests.
You should never disable firewalls, but in a controlled network environment with proper procedures established, you may find that temporarily disabling or bypassing a security appliance resolves a connectivity issue. The remedy then is to properly configure security services to allow the required connections.
```

## Network Layer

```
Various connectivity problems may also occur at the Network layer.
Important troubleshooting steps include confirming proper network names and addresses. Devices may have improperly assigned IP addresses that are causing routing issues or IP address conflicts on the network.
A device may have an improperly configured IP address because it cannot communicate with a DHCP server on the network.
Similarly, networks have different identities, such as wireless SSIDs, domain names, and workgroup names.
Another common problem exists when a particular network has conflicting names or addresses. 
Issues with DNS name resolvers may be caused by DNS caching services or connection to the wrong DNS servers. 
Internet Control Message Protocol (ICMP) is used for network control and diagnostics at the Network layer of the OSI model. Commonly used ICMP commands include ping and traceroute.
These two simple but powerful commands (and other ICMP commands and options) are some of the most commonly used tools for troubleshooting network connectivity issues.
You can run ICMP commands in the command line interface on computers, servers, routers, switches, and many other networked devices.

```

## Transport Layer

```
At the Transport layer, communications are more complex. Latency and network congestion can interfere with communications that depend on timely acknowledgments and handshakes.
Time-to-live (TTL) values sometimes have to be extended in the network service architecture to allow for slower response times during peak network traffic hours.
Similar congestion problems can occur when new services are added to an existing network or when a local device triggers a prioritized service, such as a backup or an antivirus scan.

```

## Session Layer

```
Session layer settings can also be responsible for dropped network connections. 
For example, devices that automatically go into a power standby mode (“sleep”) may have expired session tokens that fail when the device attempts to resume connectivity. 
At the server, failover communications or handshake negotiations with one server may not translate to other clustered servers. Sessions may have to be restarted.
```
## Presention Layer

```
Presentation layer conflicts are often related to changes in encryption keys or updates to service architectures that are not supported by various client devices.
For example, an older browser may not interoperate with a script or a new encoding standard.
```

## Application Layer

```
Application layer network connectivity problems are extremely common. Many applications may conflict with other apps. 
Apps also may have caching or corrupted files that can be remedied only by uninstalling and reinstalling or by updating to a newer version. 
Some apps also require persistent connections to update services or third parties, and network security settings may prevent those connections from being made.
```


### Example Usage

---

## 📚 Content

### 1. Physical Layer
- **Goal:** Ensure physical connectivity is working.  
- **Troubleshooting Checklist:**
  - Check for loose or damaged cables.
  - Confirm devices are powered on and receiving electricity.
  - Test wireless access points and antennas.  
- **Practical Example:**  
  A loose Ethernet cable can cause connection loss. Always start with the basics: **confirm physical connectivity**.

---

### 2. Data Link Layer
- **Goal:** Validate compatibility of link-layer standards and protocols.  
- **Troubleshooting Checklist:**
  - Confirm the device is using the correct standard (Ethernet, Wi-Fi, Bluetooth).
  - Verify encryption keys and security settings.
  - Review firewall and security policies.  
- **Practical Example:**  
  A device may lose connectivity when switching between Wi-Fi and Bluetooth. Adjust configurations to ensure compatibility.

---

### 3. Network Layer
- **Goal:** Resolve addressing and routing issues.  
- **Troubleshooting Checklist:**
  - Confirm IP addresses and subnet masks.
  - Check for IP conflicts or DHCP failures.
  - Test DNS name resolution.  
- **Useful Tools:**
  - `ping` → Tests basic connectivity.  
  - `traceroute` → Identifies the path to the destination.  
- **Practical Example:**  
  If a website doesn’t load, it may be a DNS issue. Test with `ping` using the IP directly to confirm.

---

### 4. Transport Layer
- **Goal:** Ensure communication is reliable and efficient.  
- **Troubleshooting Checklist:**
  - Analyze latency and network congestion.
  - Adjust **TTL** values when necessary.
  - Check bandwidth-heavy services (backups, antivirus scans).  
- **Practical Example:**  
  During peak hours, congestion may cause failures. Adjusting transport parameters can help stabilize connections.

---

### 5. Session Layer
- **Goal:** Manage and maintain communication sessions between devices.  
- **Troubleshooting Checklist:**
  - Verify that sessions are being established and maintained correctly.
  - Check authentication and authorization processes.
  - Ensure session timeouts are properly configured.  
- **Practical Example:**  
  If a user is repeatedly disconnected from a remote desktop session, the issue may be related to session timeout settings or improper authentication.

---

### 6. Presentation Layer
- **Goal:** Ensure data is properly formatted, encrypted, and translated for communication.  
- **Troubleshooting Checklist:**
  - Confirm that encryption/decryption settings are correct.
  - Verify data format compatibility (e.g., ASCII vs. Unicode).
  - Check compression settings if data transfer is slow.  
- **Practical Example:**  
  If a file transfer results in unreadable characters, the issue may be due to mismatched encoding formats between devices.

---

### 7. Application Layer
- **Goal:** Troubleshoot issues with applications and services that interact directly with users.  
- **Troubleshooting Checklist:**
  - Verify application configurations (e.g., email client, web browser).
  - Check for proper credentials and permissions.
  - Ensure services (HTTP, FTP, SMTP, etc.) are running and accessible.  
- **Practical Example:**  
  If a user cannot send emails, the issue may be with the SMTP server configuration or incorrect login credentials.

---

## 🎯 How to Use This Repository
- Read each section to understand how to diagnose problems at each OSI layer.  
- Apply the **checklists** in real troubleshooting scenarios.  
- Contribute with practical examples and tips via **Pull Requests**.  

---

## 🤝 Contributions
If you have experience in network troubleshooting, feel free to contribute with examples, tools, or real-world cases.  

---

## 📜 License
This project is distributed under the MIT License.  

---

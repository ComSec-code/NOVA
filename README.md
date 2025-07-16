<p align="center">
  <img src="logo.png" alt="NOVA logo" width="200">
</p>

<h1 align="center">NOVA</h1>
<p align="center"><b>New Operational Voice Architecture</b></p>
<p align="center">Sovereign, encrypted, cloud-native communications for critical operations</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Active-brightgreen">
  <img src="https://img.shields.io/badge/Kubernetes‑Ready-326CE5">
  <img src="https://img.shields.io/badge/E2E%20Encryption-Enabled-red">
  <img src="https://img.shields.io/badge/Sovereignty-Full-orange">
</p>

---

## 🚀 What is NOVA?

**NOVA** is a secure Push-to-Talk (PTT) and data communication platform, fully containerized and deployable on any Kubernetes cluster. Built for mission-critical environments that demand reliability, security, and independence.

**Key Features:**
- 🛡️ **Zero-trust communication** with end-to-end encryption
- 📶 **Hybrid connectivity** - 4G/5G, LoRa mesh, offline fallback
- 📊 **Real-time monitoring** with AI-powered threat detection
- 🛰️ **Edge deployment** for complete sovereignty

---

## 🔧 Architecture

```
nova-system/
├── ptt-server        # Encrypted WebRTC/SIP core
├── dispatcher-ui     # Command & control interface
├── auth-gateway      # Identity and access (OAuth2/SAML)
├── monitoring-stack  # Grafana · Prometheus · Loki
├── morpheus-agent    # (optional) AI threat detection
└── lora-bridge       # (optional) Mesh communications
```

**Tech Stack:** Kubernetes · Helm · Docker · WireGuard · Go · React · Grafana · eBPF

---

## 🚀 Quick Start

```bash
# Clone and deploy
git clone https://github.com/ComSec-code/NOVA.git
cd NOVA

# Install on Kubernetes
helm install nova ./deployments/helm/nova \
  --namespace nova-system --create-namespace

# Access the interface
kubectl port-forward svc/dispatcher-ui 8080:80 -n nova-system
```

**→ Open:** [http://localhost:8080](http://localhost:8080)

---

## 📖 Documentation

- **[Architecture](docs/architecture/)** - System design and components
- **[Deployment](docs/deployment/)** - Installation and configuration
- **[Operations](docs/ops/)** - Day-to-day management
- **[Security](docs/security/)** - Security model and compliance

---

## 🛰️ Strategic Edge

> **NOVA is designed for independence.**  
> No vendor lock-in. No foreign cloud. No compromise.  
> Complete control over your critical communications.

---

## 📞 Contact

**✉️ [contact@nova-comm.org](mailto:contact@nova-comm.org)**

Demo, partnership, or strategic deployment available on request.

---

<p align="center"><i>"Built for those who must communicate — when others go dark."</i></p>

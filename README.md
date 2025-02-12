# 🌐 Vyxa LLM

**Vyxa** is an **open-source large language model (LLM)** designed for **Web3 developers, AI researchers, and decentralized applications**.
It provides cutting-edge capabilities for **smart contract auditing, blockchain analytics, and DeFi automation**.

---

## ⚡ Quick Start - Run Vyxa with Ollama

Vyxa is available via **Ollama**, allowing you to run it locally with minimal setup.

### 🔹 Step 1: Install Ollama

Ollama is required to run Vyxa. Install it using the following command:

#### 🖥 macOS & Linux
```bash
curl -fsSL https://ollama.com/install.sh | sh
```

#### 🖥 Windows
Download and install from: [Ollama for Windows](https://ollama.com/download/windows)

Verify the installation:
```bash
ollama --version
```

---

### 🔹 Step 2: Download & Run Vyxa

Once Ollama is installed, pull the [Vyxa LLM](https://ollama.com/VyxaFoundation/Vyxa)  model:

```bash
ollama pull VyxaFoundation/Vyxa
```

Run the model:

```bash
ollama run VyxaFoundation/Vyxa
```
 
---

## 🔧 API Integration (Optional)

Vyxa can be used as an API to integrate AI capabilities into your applications.

### 🔹 Start the API Server
```bash
ollama serve
```

### 🔹 Make a Request via Curl
```bash
curl -X POST "http://localhost:11434/api/generate" \
     -H "Content-Type: application/json" \
     -d '{
           "model": "VyxaFoundation/Vyxa",
           "prompt": "Write a smart contract"
         }'

```

### 🔹 Example Response
```json
{
  "response": "pragma solidity ^0.8.0; contract Vyxa { ... }"
}
```

---

## ⚙️ Model Details

- **Architecture:** LLaMA-based
- **Parameters:** 70.6B
- **Quantization:** Q4_K_M (43GB)
- **License:** MIT License
- **Memory Requirement:**
  - **43GB** (Quantized)
  - **140GB** (Full Precision)

---

## 🔥 Advanced Usage

### 🔹 Running Vyxa in Interactive Mode
To chat with Vyxa in real time:

```bash
ollama run VyxaFoundation/Vyxa --interactive
```

### 🔹 Running Vyxa with a System Prompt
```bash
ollama run VyxaFoundation/Vyxa -p "Explain the impact of AI in Web3."
```

### 🔹 Running Vyxa with Custom Parameters
You can adjust **temperature, top_p, and max tokens**:

```bash
ollama run VyxaFoundation/Vyxa -t 0.7 -p "Generate Solidity code for an ERC-20 token."
```

---

## 🌍 Roadmap & Future Updates

### 🔹 Upcoming Features

✅ **Vyxa-Next** – Lightweight Model for Mobile & Edge AI  
✅ **Vyxa Chat** – AI-Powered Web3 Conversational Model  
✅ **Decentralized AI Compute** – Vyxa x Akash, Bittensor, Solana  
✅ **On-Chain AI Oracles** for Smart Contracts  

---

## 📌 Troubleshooting

🔹 **Model download is slow?**  
➡️ Use a VPN or a faster mirror.  

🔹 **Model runs out of memory?**  
➡️ Try running a lower quantization version (Q4, Q6).  

🔹 **Ollama is not recognized?**  
➡️ Ensure Ollama is installed and added to your system’s **PATH**.  

---

## Stay Connected

💻 **Website:** [Vyxa.org](https://www.vyxa.org/)  
📂 **GitHub:** [Vyxa GitHub](https://github.com/VyxaFoundation)  
𝕏 **Twitter/X:** [@VyxaFoundation](https://x.com/vyxaFoundation)

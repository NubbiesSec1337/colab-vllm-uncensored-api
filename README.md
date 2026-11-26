# Colab vLLM Uncensored API

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/NubbiesSec1337/colab-vllm-uncensored-api/blob/main/colab-vllm-uncensored-api.ipynb)

Notebook Google Colab untuk menjalankan model LLM uncensored (Dolphin, Qwen Abliterated, Llama Abliterated, Hermes) menggunakan **vLLM** sebagai **OpenAI-compatible API** (`/v1/chat/completions`) yang di-expose lewat **Cloudflare Tunnel** (`cloudflared`) dengan proteksi **API Key**.

## Pilihan GPU & Preset Model

| GPU Colab | VRAM | Preset Model di Dropdown |
| :--- | :---: | :--- |
| **L4 / A100** | 24 GB+ | `Dolphin3.0-Mistral-24B-AWQ`, `Dolphin3.0-R1-Mistral-24B-AWQ`, `Huihui-Qwen3.6-27B-abliterated-AWQ`, `Qwen3-32B-abliterated-awq` |
| **A100 / H100** | 40 GB+ | `Dolphin-Mistral-24B-Venice-Edition-FP8`, `Huihui-Qwen3.8-27B-abliterated-FP8` |
| **H100** | 80 GB | `llama3.3-70B-instruct-abliterated-awq`, `Hermes-4-70B-AWQ-4bit`, `Llama-3.3-70B-Instruct-abliterated-FP8`, `Hermes-3-Llama-3.1-70B-FP8` |

## Cara Pakai

1. Klik tombol **Open In Colab** di atas.
2. Pilih GPU di **Runtime → Change runtime type** (**L4**, **A100**, atau **H100**).
3. Pilih model di dropdown **Step 2** (atau isi `CUSTOM_MODEL_ID` dengan repo Hugging Face lain).
4. Klik **Runtime → Run all**.
5. Salin **Base URL**, **API Key**, dan **Model Name** dari output **Step 4**.
6. Setelah selesai, klik **Runtime → Disconnect and delete runtime** agar Compute Units tidak terus terpakai.

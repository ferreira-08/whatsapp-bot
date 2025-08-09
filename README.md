# 🤖 Bot de Envio de Mensagens via WhatsApp Web

Este projeto automatiza o envio de mensagens personalizadas via WhatsApp Web, utilizando Python e leitura de dados de uma planilha Excel.

## 🚀 Funcionalidades

- Leitura de contatos a partir de uma planilha `.xlsx`
- Envio automático de mensagens via WhatsApp Web
- Mensagens personalizadas com nome e data de vencimento
- Registro de envios bem-sucedidos e erros em arquivos `.csv`

## 🛠️ Tecnologias Utilizadas

- Python 3.10+
- `openpyxl`
- `webbrowser`
- `urllib.parse`
- `time`, `os`, entre outras

## 📁 Estrutura dos Arquivos
whatsapp-bot/ ├── bot_wpp.py # Código principal do bot
├── clientes.xlsx # Planilha com os dados dos clientes
├── sucesso.csv # Log de mensagens enviadas com sucesso 
├── erros.csv # Log de erros no envio 
└── README.md # Este arquivo


## 📝 Formato da Planilha (`clientes.xlsx`)

A planilha deve conter as seguintes colunas:

| nome   | telefone     | vencimento   |
|--------|--------------|--------------|
| João   | 55999999999  | 10/08/2025   |
| Maria  | 55988888888  | 11/08/2025   |

## ⚙️ Como Usar

1. Instale o Python 3.10 ou superior.
2. Instale a biblioteca `openpyxl`:
   ```bash
   pip install openpyxl
   python bot_wpp.py

O navegador será aberto com o WhatsApp Web. Escaneie o QR Code.

O bot começará a enviar as mensagens automaticamente.

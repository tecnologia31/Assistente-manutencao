# 🛠️ Assistente de Manutenção Inteligente para Perfuratriz Autônoma

Este projeto é um assistente de manutenção que utiliza Inteligência Artificial (IA) e Busca Semântica para encontrar soluções em **manuais técnicos em inglês** e traduzir as instruções diretamente para o **português**. É ideal para técnicos que precisam de acesso rápido a informações de diagramas e procedimentos em campo.

## 🚀 Como Usar o Assistente (Site Hospedado)

O assistente está disponível online e não requer nenhuma instalação.

1.  Acesse o link da aplicação: [**INSIRA AQUI O LINK DO SEU HUGGING FACE SPACE**]
2.  No menu suspenso, selecione o modelo da perfuratriz que você está reparando (ex: `MD6420`, `MD6310`, ou `PV275`).
3.  Na caixa de texto, **descreva a falha em português** (ex: "O sistema hidráulico não pressuriza" ou "O display mostra erro E102").
4.  O sistema retornará a solução traduzida e a **imagem completa da página do manual original** para referência visual.

## ⚙️ Modelos de Perfuratriz Suportados

Os seguintes modelos possuem seus manuais carregados no sistema:
* **MD6420**
* **MD6310**
* **PV275**

---

## 💻 Configuração e Desenvolvimento (Para Administradores)

### 1. Requisitos

O projeto é baseado em Python e usa as seguintes bibliotecas, listadas em `requirements.txt`:
* `gradio` (Interface Web)
* `PyPDF2`, `pdf2image` (Processamento de PDFs)
* `sentence-transformers` (Busca Semântica com IA)
* `googletrans` (Tradução)

Além das bibliotecas Python, é necessária a biblioteca de sistema operacional **`poppler-utils`** para a conversão de PDF para imagem.

### 2. Estrutura de Pastas

Para que o assistente funcione corretamente, os manuais em PDF (em inglês) devem estar organizados na pasta `manuals/` da seguinte forma:

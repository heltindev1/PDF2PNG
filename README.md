# 📸 PDF2PNG - Conversor de PDF para Imagem

Este projeto é uma ferramenta em Python desenvolvida para automatizar a extração de imagens de arquivos PDF.  
Ele transforma cada página de um documento PDF em um arquivo de imagem individual (PNG), mantendo alta resolução e fidelidade visual.

---

# 🛠️ Pré-requisitos

Antes de iniciar, certifique-se de ter instalado em seu ambiente:

## 1. Python
Baixe aqui: https://www.python.org/downloads/  
Durante a instalação marque a opção **"Add Python to PATH"**.

## 2. Visual Studio Code (Opcional)
Recomendado para edição e execução do script.  
Baixe aqui: https://code.visualstudio.com/

---

# 🚀 Guia de Configuração e Uso

## 1. Instalação de Dependências

O script utiliza a biblioteca **PyMuPDF**.

Abra o terminal (CMD ou PowerShell) e execute:

```bash
pip install pymupdf
```

---

## 2. Configuração de Diretórios (Caminhos)

Este código é livre e genérico.  
Você deve indicar os diretórios de origem e destino editando o arquivo **main.py**.

### ⚠️ IMPORTANTE

Você precisa alterar os caminhos abaixo no código para que o script encontre seus arquivos.

Localize o bloco de configuração no `main.py` e insira seus caminhos locais:

```python
# =================================================================
# CONFIGURAÇÃO DE CAMINHOS - CAMINHO EXPLICITO PARA ALTERAÇÃO
# =================================================================

# Insira o caminho da pasta onde estão os arquivos PDF originais
PASTA_ORIGEM = r'C:\CAMINHO\DA\SUA\PASTA\DE\ORIGEM'

# Insira o caminho da pasta onde as imagens convertidas serão salvas
PASTA_DESTINO = r'C:\CAMINHO\DA\SUA\PASTA\DE\DESTINO'

# =================================================================
```

### 💡 Dica

O prefixo **r** antes das aspas é necessário no Windows para que o interpretador processe corretamente as barras invertidas (`\`) dos diretórios.

---

# 💻 Métodos de Execução

## Via Terminal (Prompt de Comando / CMD)

1. Navegue até a pasta onde o arquivo `main.py` está localizado.
2. Na barra de endereços do explorador de arquivos digite:

```
cmd
```

3. No terminal execute:

```bash
python main.py
```

---

## Via Visual Studio Code (VS Code)

1. Abra a pasta do projeto no VS Code (`File > Open Folder`).
2. Selecione o arquivo `main.py`.
3. Clique em **Run Python File (▷)** no canto superior direito  
   ou pressione **F5**.

---

# 📂 Detalhes do Processamento

## Varredura Automática
O script identifica todos os arquivos com extensão `.pdf` no diretório de origem indicado.

## Gestão de Pastas
Caso o diretório de destino não exista, o sistema o cria automaticamente.

## Escalonamento de Imagem
A conversão utiliza uma matriz **2.0x (DPI elevado)**, garantindo nitidez para textos e elementos gráficos.

## Padronização de Saída
Os arquivos PNG são nomeados seguindo o padrão:

```
nome_original_pag_X.png
```

---

# ⚠️ Segurança e Privacidade

## Execução Local
O processamento ocorre integralmente no hardware local.  
Nenhum dado é transmitido para servidores externos.

## Transparência
O código está aberto para auditoria de segurança e integridade de dados.

---

# ✒️ Autor

Desenvolvido por **Helton (heltindev)**

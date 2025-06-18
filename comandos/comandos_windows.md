# ⚙️ Comandos de Prompt de Comando (CMD) - Windows

⚠️ **Todos os comandos foram testados no Windows 10.**

---

## 🗓️ Data e Hora

- **Exibir a data atual:**
```bash
date
```

- **Exibir a hora atual:**
```bash
time
```

---

## 📂 Diretórios e Arquivos

- **Exibir o diretório atual:**
```bash
echo %cd%
```

- **Listar arquivos e pastas do diretório atual:**
```bash
dir
```

---

## 🗑️ Exclusão de Arquivos e Pastas

- **Deletar um arquivo:**
```bash
del nome_do_arquivo.extensao
```

---

- **Deletar uma pasta vazia:**
```bash
rmdir nome_da_pasta
```

---

- **Deletar uma pasta que não esteja vazia:**
```bash
rmdir /s nome_da_pasta
```

---

## 📜 Visualizar Conteúdos

- **Exibir o conteúdo de um arquivo:**
```bash
type nome_do_arquivo.extensao
```
---

## 🧽 Limpar o Terminal

- **Limpar a tela do terminal:**
```bash
cls
```

---

✔️ *Esses são comandos essenciais para navegação, manipulação e organização de arquivos e diretórios no Windows via terminal CMD.*

# 🔧 Comandos Avançados do CMD - Windows

## 1. 🔍 SFC (Verificar Integridade dos Arquivos do Sistema)

O comando `sfc /scannow` realiza uma varredura completa no sistema para identificar e reparar arquivos corrompidos do Windows.
```bash
sfc /scannow
```

📄 **Observação:** Ao finalizar, o sistema exibirá um relatório informando se houve ou não problemas encontrados e corrigidos.

---
## 2. 📁 Robocopy (Cópia Avançada de Arquivos)

Permite realizar cópias robustas de arquivos e pastas, sendo muito utilizado para backup.

```bash
robocopy "C:\pasta_origem" "C:\pasta_destino"
```

## 3. ℹ️ Systeminfo (Informações do Sistema)

Exibe informações detalhadas sobre o sistema operacional, incluindo data de instalação, fabricante, versão, memória, entre outros.

```bash
systeminfo
```

---
## 4. ❌ Taskkill (Finalizar Processos)

Força o encerramento de um programa ou processo específico.

```bash
taskkill /f /im nome_do_programa.exe
```
## 5. 📃 Tasklist (Listar Processos em Execução)

Mostra todos os processos ativos no momento, semelhante ao Gerenciador de Tarefas, porém com mais detalhes no terminal.

```bash
tasklist
```

---

## 6. 🔌 Shutdown (Desligar ou Reiniciar o Computador)

- **Desligar o computador:**
```bash
shutdown -s -t 300
```
➡ Desliga em 5 minutos (300 segundos).

- **Reiniciar o computador:**
```bash
shutdown -r -t 300
```

---
## 7. 🌐 Ipconfig (Informações de Rede)

Exibe detalhes da configuração de rede, como IP, máscara de sub-rede e gateway.

```bash
ipconfig /all
```

---

## 8. 📄 Assoc (Associação de Extensões)

Mostra ou define qual programa está associado a uma extensão de arquivo.

```bash
assoc .extensao
```
## 9. 🖥️ Driverquery (Listagem de Drivers)

Exibe uma lista de todos os drivers instalados no sistema.

```bash
driverquery -v
```

---

## 10. 🔍 Fc (Comparar Arquivos)

Compara dois arquivos e retorna as diferenças entre eles.

```bash
fc /c caminho_do_arquivo1 caminho_do_arquivo2
```
✔️ *Esses comandos são extremamente úteis tanto para manutenção quanto para diagnósticos e automação no Windows.*
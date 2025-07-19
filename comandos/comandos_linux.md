# ⚙️ Comandos Essenciais de Terminal – Linux

⚠️**Todos os comandos foram testados em Kali Linux (Debian‑based).**

---

## 🗓️ Data e Hora

- **Exibir a data e hora:**
```bash
$ date
seg 14 jul 2025 09:16:40 CST
```

- **A opção “-u” mostra as horas no formato UTC:**
```bash
$ date -u
seg 14 jul 2025 15:18:01 UTC
```

---

## 📂 Diretórios e Arquivos

- **Exibir o diretório atual:**
```bash
$ pwd
```

- **Listar arquivos e pastas do diretório atual:**
```bash
$ ls
```

---

## 🗑️ Exclusão de Arquivos e Pastas

- **Deletar um arquivo:**
```bash
$ rm nome_do_arquivo
```

---

- **Deletar uma pasta vazia:**
```bash
$ rmdir nome_da_pasta
```

---

- **Deletar uma pasta que não esteja vazia:**
```bash
$ rm -r nome_da_pasta
```

---

## 📜 Visualizar Conteúdos

- **Exibir o conteúdo de um arquivo:**
```bash
$ cat nome_do_arquivo
```
---

## 🧽 Limpar o Terminal

- **Limpar a tela do terminal:**
```bash
$ clear
```

---

✔️ *Esses são comandos essenciais para navegação, manipulação e organização de arquivos e diretórios no Linux via terminal Bash.*

# 🔧 Comandos Avançados do Linux

## 1.  🐧 Atualização de Pacotes (APT)

- **Atualizar lista de pacotes:**
```bash
sudo apt update

```
- **Atualizar pacotes instalados:**
```bash
sudo apt upgrade


```
- **Instalar um pacote:**
```bash
sudo apt install nome_do_pacote
```


---
## 2. 📁 Cópia Avançada de Arquivos

`rsync` é amplamente usado em sistemas Linux para backups e sincronização de arquivos.

```bash

$rsync -avh "/home/usuario/Área de trabalho/teste/" "/home/usuario/Backup/"

```

## 3. ℹ️ Systeminfo (Informações do Sistema)

Exibe informações sobre o sistema, incluindo data de instalação, fabricante, versão, memória, entre outros.

```bash
$ uname -a
```
Para mim, o sistema retornou
```bash
Linux kaliRecon 6.12.25-amd64 #1 SMP PREEMPT_DYNAMIC Kali 6.12.25-1kali1 (2025-04-30) x86_64 GNU/Linux
```

O primeiro item é o nome do Kernel do sistema. Para que seja mostrado na tela apenas ele, digite:

```bash
$ uname
```

---
## 4. ❌ Taskkill (Finalizar Processos)

Usar o comando pkill
O pkill permite encerrar processos a partir de seus nomes, em vez de PIDs:


```bash
$pkill nome_do_processo
```
Com força :
```
 $pkill -9 nome_do_processo
 ```

## 5. 📃 Tasklist (Listar Processos em Execução)

Mostra todos os processos ativos no momento, semelhante ao Gerenciador de Tarefas, porém com mais detalhes no terminal.

```bash
$ps aux
```

---

## 6. 🔌 Shutdown (Desligar ou Reiniciar o Computador)

- **Desligar o computador:**
```bash
sudo shutdown -h +5
```
➡ Desliga em 5 minutos (300 segundos).

- **Reiniciar o computador:**
```bash
sudo shutdown -r +5
```
➡ Renicia em 5 minutos 

---
## 7. 🌐 Ipconfig (Informações de Rede)

Exibe detalhes da configuração de rede, como IP, máscara de sub-rede e gateway.

```bash
ip a
```

---

## 8. 📄 Assoc (Associação de Extensões)

Mostra o tipo MIME associado a um determinado arquivo no sistema Linux.

```bash
xdg-mime query filetype arquivo.ext
```
## 9. 🖥️ Driverquery (Listagem de Drivers)

Exibe uma lista de todos os drivers instalados no sistema.

```bash
lshw -short
```
ou
```bash
sudo lspci
sudo lsmod
```

---

## 10. 🔍 Fc (Comparar Arquivos)

Compara dois arquivos e retorna as diferenças entre eles.

```bash
diff arquivo1 arquivo2
```
✔️ *Esses comandos são essenciais tanto para manutenção quanto para diagnósticos em sistemas Linux.*
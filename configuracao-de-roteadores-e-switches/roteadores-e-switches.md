# 🔧 Configuração de Roteadores e Switches (Packet Tracer, NetAcad)

## 📘 Conceitos Básicos

- **Roteador (Router):** Dispositivo que conecta diferentes redes e encaminha pacotes entre elas, geralmente utilizando endereçamento IP.
- **Switch:** Dispositivo de comutação usado em redes locais (LAN) que conecta dispositivos e encaminha quadros com base no endereço MAC.

---

## 🧠 Etapas Gerais de Configuração

### 1. Acesso ao Equipamento
- **Console:** Acesso direto via cabo console.
- **Telnet/SSH:** Acesso remoto (necessita configuração prévia).

### 2. Modo Privilegiado
```bash
enable
```

### 3. Modo de Configuração Global
```bash
configure terminal
```

---

## 🌐 Configuração de Roteador no Packet Tracer

### ✅ Definir nome do roteador
```bash
hostname R1
```

### ✅ Configurar interface (exemplo: FastEthernet 0/0)
```bash
interface fa0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
exit
```

### ✅ Ativar protocolo de roteamento (ex: RIP)
```bash
router rip
network 192.168.1.0
exit
```

---

## 🧩 Configuração de Switch

### ✅ Definir nome do switch
```bash
hostname SW1
```

### ✅ Criar VLAN
```bash
vlan 10
name VENDAS
exit
```

### ✅ Atribuir porta a uma VLAN
```bash
interface fa0/1
switchport mode access
switchport access vlan 10
exit
```

---

## 🔐 Configurações de Segurança

### ✅ Senha no modo privilegiado
```bash
enable secret senha123
```

### ✅ Senha para acesso via console
```bash
line console 0
password console123
login
exit
```

### ✅ Senha para acesso remoto (VTY)
```bash
line vty 0 4
password remoto123
login
exit
```

---

## 💻 Comandos Úteis de Verificação

| Comando                    | Descrição                                   |
|----------------------------|---------------------------------------------|
| `show ip interface brief` | Exibe as interfaces e IPs configurados      |
| `show vlan`               | Mostra as VLANs criadas no switch           |
| `show running-config`     | Mostra todas as configurações ativas        |
| `ping <IP>`               | Testa a conectividade com outro dispositivo |

---

## 🧪 Exemplo de Topologia no Packet Tracer

1. Um roteador (R1) conectado a dois switches (SW1 e SW2).
2. Cada switch conectado a dois PCs.
3. VLANs: VLAN 10 (Administração) e VLAN 20 (Financeiro).
4. IPs estáticos atribuídos a cada PC.
5. Testar conectividade usando o comando `ping` entre dispositivos da mesma VLAN e com o gateway (roteador).

---

## 📚 Dicas do NetAcad

- Utilize os laboratórios do **Cisco Networking Academy** para praticar configurações reais.
- Salve suas topologias no Packet Tracer e anote os comandos usados.
- Use o **modo simulação** do Packet Tracer para entender o caminho dos pacotes.

---
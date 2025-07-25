# 📡 Endereçamento IPv4 - Conceitos Básicos

O endereçamento IPv4 é um dos fundamentos essenciais das redes de computadores. Cada dispositivo conectado a uma rede precisa de um endereço IP para se comunicar.

---

## 🔢 Estrutura de um Endereço IPv4

Um endereço IPv4 possui 32 bits, divididos em 4 blocos de 8 bits (octetos), normalmente representados em decimal separados por pontos.  
Exemplo: `192.168.1.1`

---

## 🧩 Classes de Endereços IPv4

Os endereços IPv4 são divididos em **classes**, de acordo com o valor do primeiro octeto. Essa divisão facilita o roteamento e a organização das redes.

| Classe | Intervalo do 1º Octeto | Intervalo de IPs             | Máscara Padrão     | Uso comum                        |
|--------|------------------------|------------------------------|--------------------|----------------------------------|
| A      | 1 a 126                | 1.0.0.0 a 126.255.255.255    | 255.0.0.0 (/8)     | Grandes redes (empresas)        |
| B      | 128 a 191              | 128.0.0.0 a 191.255.255.255  | 255.255.0.0 (/16)  | Redes médias (universidades)    |
| C      | 192 a 223              | 192.0.0.0 a 223.255.255.255  | 255.255.255.0 (/24)| Pequenas redes (residenciais)   |
| D      | 224 a 239              | 224.0.0.0 a 239.255.255.255  | Multicast          | Transmissão de dados em grupo   |
| E      | 240 a 255              | 240.0.0.0 a 255.255.255.255  | Reservado          | Uso experimental / testes       |

> ⚠️ O endereço `127.0.0.1` pertence ao **loopback** (teste local) e não se encaixa nas classes tradicionais.

---

## 📍 Endereços Privados

São usados para redes internas e não são roteáveis pela internet. Reservados nas classes A, B e C:

- **Classe A:** `10.0.0.0 – 10.255.255.255`
- **Classe B:** `172.16.0.0 – 172.31.255.255`
- **Classe C:** `192.168.0.0 – 192.168.255.255`

---

## 🧮 Máscaras de Sub-rede

A máscara de sub-rede define a **parte da rede** e a **parte do host** em um IP. Exemplo:

- IP: `192.168.1.10`
- Máscara: `255.255.255.0` → rede: `192.168.1.0`

---

## 🔍 CIDR e Notação de Prefixo

A notação **CIDR (Classless Inter-Domain Routing)** usa a barra `/` para indicar quantos bits são da rede.

- `192.168.1.0/24` → 24 bits para rede, 8 bits para host

---

## ✍️ Recomendações

- Utilize o comando `ipconfig` (Windows) ou `ifconfig` / `ip a` (Linux) para verificar seu IP.
- Planeje bem o **subnetting** para evitar desperdício de endereços.

---

🔗 Baseado em [youstable.com](https://www.youstable.com/blog/ipv4-address-classes) e exercícios de subnetting da Cisco.


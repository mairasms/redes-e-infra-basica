# 🌐 Introdução ao IPv6

O **IPv6 (Internet Protocol version 6)** é a versão mais recente do protocolo IP, criado para substituir o IPv4, que está se esgotando devido ao número crescente de dispositivos conectados à internet.

---

## 📘 O que é IPv6?

O IPv6 é o protocolo de endereçamento que permite que dispositivos se comuniquem em redes IP. Ele foi projetado para resolver as limitações do IPv4, principalmente o número limitado de endereços.

---

## 📊 Diferenças entre IPv4 e IPv6

| Característica        | IPv4                          | IPv6                                  |
|-----------------------|-------------------------------|----------------------------------------|
| Comprimento do endereço | 32 bits                      | 128 bits                               |
| Representação         | Decimal (ex: 192.168.0.1)     | Hexadecimal (ex: 2001:0db8::1)         |
| Quantidade de endereços | ~4,3 bilhões                 | ~340 undecilhões (3.4 × 10³⁸)          |
| Configuração automática | Limitada (via DHCP)         | Nativa (Stateless Address Autoconfig)  |
| Segurança integrada    | Opcional                     | IPsec obrigatório                      |
| Suporte a QoS          | Limitado                     | Avançado                               |

---

## ✅ Vantagens do IPv6

- 🌍 **Número quase infinito de endereços IP**
- 🔐 **Segurança nativa com IPsec**
- ⚡ **Maior desempenho e eficiência no roteamento**
- 🔧 **Autoconfiguração de dispositivos**
- 🚀 **Suporte aprimorado a mobilidade e IoT**

---

## ⚠️ Desvantagens

- 🔄 Nem todos os dispositivos ou provedores oferecem suporte total.
- 🕸️ Alguns sites ainda não funcionam com IPv6 puro.
- 🔧 Requer atualização de hardware (roteadores e modems compatíveis).
- 🌐 Pode exigir conhecimento técnico para configuração inicial.

---

## 🔧 Formato de um Endereço IPv6

Um endereço IPv6 tem **128 bits** e é representado por **8 grupos de 4 dígitos hexadecimais**, separados por dois-pontos:
Exemplo: 2001:0db8:85a3:0000:0000:8a2e:0370:7334


> Dicas:
> - Zeros à esquerda podem ser omitidos.
> - Sequências contínuas de zeros podem ser substituídas por `::` **uma vez** por endereço.

---

## 🌐 Métodos de Conexão IPv6

- **DHCPv6**: atribuição automática pelo provedor.
- **Stateless** (SLAAC): configuração automática sem servidor.
- **6to4 / Tunnel Broker**: para redes IPv6 sobre IPv4.
- **IPoE vs PPPoE**:
  - *PPPoE* (IPv4): conexão via autenticação.
  - *IPoE* (IPv6): conexão direta e mais rápida (sem autenticação manual).

---

## 🚀 Exemplo de configuração básica (DHCPv6)

1. Acesse o painel do seu roteador (ex: `192.168.0.1`)
2. Vá para **Configurações de Rede > IPv6**
3. Escolha o tipo de conexão: `DHCPv6`
4. Insira as informações fornecidas pelo provedor (Prefixo, Gateway, DNS)
5. Salve e reinicie o roteador

---

## 🔐 Segurança

O IPv6 possui recursos nativos de segurança, como IPsec. Ainda assim, é importante:
- Manter o firmware atualizado
- Usar senhas fortes
- Configurar corretamente firewall e portas

---

## 🔍 Teste seu IPv6

Use ferramentas online para verificar se seu dispositivo está usando IPv6:
[https://test-ipv6.com](https://test-ipv6.com)

---

📚 Fontes:
- HogoNext: *How to Configure IPv6 on Your Router*
- NTT Japan: *IPv6 - Benefícios e Diferenças com IPv4*



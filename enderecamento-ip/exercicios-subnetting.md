# 📚 Exercícios de Subnetting

A seguir, alguns exemplos práticos para fixar o conceito de sub-redes.

---

## 🧪 Exemplo 1 — Quantas sub-redes posso criar?

**Rede base:** `192.168.1.0/24`  
**Nova máscara desejada:** `/26`

- Bits emprestados: `26 - 24 = 2`
- Sub-redes possíveis: `2² = 4`
- Hosts por sub-rede: `2⁶ - 2 = 62`

**Sub-redes criadas:** <details> <summary> Clique aqui para ver a resposta</summary>





    192.168.1.0 - 192.168.1.63

    192.168.1.64 - 192.168.1.127

    192.168.1.128 - 192.168.1.191

    192.168.1.192 - 192.168.1.25

</details>

---

## 🧪 Exemplo 2 — Qual a máscara para 50 hosts?

**Rede base:** `10.0.0.0`  
**Número de hosts por sub-rede:** `50`

- Fórmula: `2ⁿ - 2 ≥ 50` → `n = 6`
- Bits para host: 6 → bits para rede: `32 - 6 = 26`
- Máscara: `/26` → `255.255.255.192`

---

## 🧪 Exemplo 3 — Qual o intervalo da sub-rede?

**IP:** `192.168.10.130`  
**Máscara:** `/27` → `255.255.255.224`

- Bloco: `2⁵ = 32`
- 130 está no intervalo que começa em `192.168.10.128`

Rede: 192.168.10.128
Broadcast:192.168.10.159
Válidos: 129 a 158


---

## 💡 Dica Cisco (baseada no PDF)

No subnetting Cisco:
- Sempre verifique **quantas redes e quantos hosts** são realmente necessários
- Use a tabela de blocos (`/25 = bloco de 128`, `/26 = 64`, etc.)
- Tente memorizar as máscaras até `/30`

---

Pratique com simuladores como o **Packet Tracer**!


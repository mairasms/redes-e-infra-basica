# 🎭 Máscara de Sub-rede

A máscara de sub-rede define **qual parte do endereço IP representa a rede** e **qual representa os hosts**. Isso é essencial para dividir redes e organizar melhor o tráfego.

---

## 📌 Conceito

A máscara de sub-rede é um conjunto de 32 bits que acompanha um endereço IPv4. Ela **especifica quantos bits são usados para identificar a rede** e **quantos para identificar os hosts**.

Por exemplo:

IP: 192.168.1.10

Máscara: 255.255.255.0


Neste caso, os **24 primeiros bits** são da **rede** e os últimos **8 bits** são para os **hosts**.

---

## 🔢 Máscaras Padrão por Classe

| Classe | Máscara Padrão      | CIDR  | Nº Máximo de Hosts |
|--------|----------------------|-------|----------------------|
| A      | 255.0.0.0            | /8    | 16.777.214           |
| B      | 255.255.0.0          | /16   | 65.534               |
| C      | 255.255.255.0        | /24   | 254                  |

> Lembre-se: sempre subtrai 2 (rede + broadcast)

---

## 🧠 CIDR (Classless Inter-Domain Routing)

O CIDR usa a notação `/` para indicar o número de bits usados para a **rede**.

| CIDR | Máscara              | Nº Sub-redes (em /24) | Hosts por sub-rede |
|------|----------------------|------------------------|---------------------|
| /25  | 255.255.255.128      | 2                      | 126                 |
| /26  | 255.255.255.192      | 4                      | 62                  |
| /27  | 255.255.255.224      | 8                      | 30                  |
| /28  | 255.255.255.240      | 16                     | 14                  |
| /29  | 255.255.255.248      | 32                     | 6                   |
| /30  | 255.255.255.252      | 64                     | 2                   |

---

## 🧪 Fórmulas úteis

- **Total de sub-redes** = 2ⁿ (n = bits emprestados da parte de host)
- **Total de hosts** = 2ʰ - 2 (h = bits restantes para host)

---

## 🛠️ Aplicação prática

> Se você tem a rede `192.168.1.0/24` e quer dividir em 4 sub-redes:

- Precisamos de 2 bits extras: `2² = 4 sub-redes`
- Nova máscara: `/26` ou `255.255.255.192`
- Cada sub-rede terá 64 endereços (62 hosts válidos)




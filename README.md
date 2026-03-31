# network-infrastructure-empresa
Projeto de infraestrutura de rede corporativa com NAT, ACL, DHCP, DNS e interconexão entre filiais.

# 🌐 Projeto de Rede Corporativa – Empresa XYZ

## 📄 INTRODUÇÃO
Infraestrutura de rede corporativa para uma empresa de pequeno/médio porte, com interconexão entre duas filiais (New York e Miami).  
A rede possui serviços internos, controle de acesso por meio de ACLs e saída para rede externa simulada utilizando NAT.

---

## 🌐 TOPOLOGIA
- 2 Roteadores (conexão WAN entre filiais)
- 2 Switches (redes LAN)
- 3 Dispositivos finais (PCs e laptop)
- 2 Servidores (serviços internos)
  - Server0: DHCP
  - Server1: DNS + HTTP

---

## ⚙️ TECNOLOGIAS UTILIZADAS
- Roteamento estático
- DHCP e DHCP Relay
- DNS (resolução de nomes internos)
- HTTP Server
- ACL (controle de acesso)
- NAT (PAT com overload)

---

## 🔐 SEGURANÇA DA REDE
- ACL bloqueia o acesso da filial Miami ao Server0
- Controle de tráfego entre redes
- Separação lógica entre as redes

---

## 🧠 DESAFIOS ENFRENTADOS
- Conflito de comunicação HTTP entre filiais, apesar de conectividade ICMP funcional
- Identificação de interferência do NAT no tráfego interno
- Correção utilizando NAT Exemption (ACL específica para NAT)

---

## ✅ RESULTADO
- Comunicação completa entre filiais
- Serviços internos operacionais (DHCP, DNS, HTTP)
- NAT funcionando corretamente
- Controle de acesso aplicado com sucesso

---

## 👨‍💻 Autor
Projeto desenvolvido por Nalberty Meneses

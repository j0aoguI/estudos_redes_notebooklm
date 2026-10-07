# Contexto e objetivo
Este repositório faz parte de um estudo direncionado ao aprofundamento em Redes de Computadores, utilizando
Inteligência Artificial como ferramenta de apoio à aprendizagem e organização do conhecimento.

O interesse pelo tema surgiu a partir do meu objetivo de construir uma base sólida para posteriormente me aprofundar
em Segurança Computacional e Cibersegurança.

A compressão de redes é fundamental para entender como computadores, servidores, aplicações e dispositivos se comunicam
e, consequentemente, como vulnerabilidades e ataques podem ocorrer nesses ambientes.

# Objetivos 
- Compreender os principais conceitos de Redes de Computadores;
- Entender os modelos OSI e TCP/IP;
- Estudar os principais protocolos de comunicação;
- Compreender endereçamento IPv4 e IPv6;
- Aprender conceitos de subnetting;
- Entender o funcionamento de TCP e UDP;
- Estudar DNS, DHCP, HTTP/HTTPS, ARP e ICMP;
- Compreender roteamento, NAT e firewalls;
- Utilizar ferramentas de análise de redes;
- Relacionar os conceitos de redes com Segurança da Informação e Cibersegurança;
- Construir uma base para estudos futuros em Pentest, Blue Team, SOC e Segurança de dados

# Fontes
- https://www.cisco.com/c/pt_br/solutions/small-business/resource-center/networking/networking-basics.html#~access-points
- https://www.rfc-editor.org/rfc/rfc9293.pdf
- https://www.rfc-editor.org/info/rfc768/
- https://www.rfc-editor.org/info/rfc8200/
- https://youtu.be/3b_TAYtzuho?si=q4qm-O2sn20EscXU
- https://www.youtube.com/watch?v=2QGgEk20RXM&list=PLBbU9-SUUCwUyqvfypPAHWOaDr7Wz4P6t
- https://www.youtube.com/watch?v=kP1kktlbUTs&pp=ygUPZ2xhdWtvIGNhcnZhbGhv

# Conteúdos estudos
1. Fundamentos de Redes
2. Modelo OSI e TCP/IP
3. Endereçamento IP
4. TCP e UDP
5. DNS e DHCP
6. Roteamento
7. Segurança de Redes

# Engenharia de prompts
Durante o desenvolvimento deste projeto, utilizei o NotebookLM como ferramenta de apoio ao aprendizado. Os prompts foram 
elaborados com o objetivo de obter explicações, comparações, exemplos práticos e exercícios relacionados aos conceitos de 
Redes de Computadores.

A estratégia utilizada foi começar com perguntas mais gerais e, posteriormente, criar perguntas mais específicas para 
aprofundar os conceitos que apresentaram maior dificuldade.

**Prompt 1 — Criando uma trilha de estudos**
"Estou estudando Redes de Computadores com o objetivo de construir uma base
sólida para posteriormente estudar Segurança Computacional e Cibersegurança.

Com base nas fontes disponíveis, organize uma trilha de estudos progressiva,
começando pelos conceitos fundamentais e avançando para conceitos relacionados
à segurança de redes.

Indique a ordem recomendada dos assuntos e explique por que cada etapa é
importante para a próxima."
Objetivo: organizar os conteúdos e compreender uma sequência lógica de estudos

**Resumo da resposta obtida**
O NotebookLM organizou os estudos em seis etapas progressivas:

1. **Fundamentos de redes:** conceitos de comunicação, protocolos, dispositivos, meios físicos, Ethernet e endereçamento MAC.
2. **Modelos de rede:** estudo dos modelos OSI e TCP/IP, PDUs, encapsulamento e diagnóstico por camadas.
3. **Camada de rede:** IPv4, IPv6, DHCP, ARP, roteamento e protocolos como OSPF e BGP.
4. **Camada de transporte:** portas, TCP e UDP, incluindo handshake, estados, confiabilidade e controle de fluxo.
5. **Camada de aplicação:** modelo cliente-servidor e protocolos como DNS, HTTP/HTTPS, FTP, SMTP, POP3 e IMAP.
6. **Segurança de redes:** estudo de vulnerabilidades, ataques e mecanismos de defesa relacionados aos protocolos, incluindo spoofing, SYN Flood, análise de tráfego, IPsec, TLS, SSH e firewalls.

**Resultado obtido:**

A resposta ajudou a definir uma sequência lógica de aprendizagem, começando pelos fundamentos de redes e avançando gradualmente até Segurança de Redes. Essa organização será utilizada como base para orientar os próximos estudos.

# Cicatrizes do aprendizado
## Dificuldade 1 — TCP x UDP

Durante o estudo, tive dificuldade inicialmente para diferenciar TCP e UDP e entender por que um protocolo mais simples como o UDP é utilizado em determinadas aplicações.

A comparação mostrou que o TCP é orientado à conexão, utilizando o 3-Way Handshake, e oferece maior confiabilidade, garantindo a entrega e a ordem dos dados, além de possuir mecanismos de controle de fluxo e congestionamento. Por isso, é utilizado em aplicações como navegação Web, e-mail e transferência de arquivos.

Já o UDP não estabelece conexão e não garante a entrega ou a ordem dos dados. Por possuir menos mecanismos de controle e um cabeçalho menor, apresenta menor overhead e pode oferecer menor latência. É utilizado em aplicações como VoIP, streaming e alguns protocolos de rede, como DNS e DHCP.

Principal aprendizado: percebi que TCP não é simplesmente "melhor" que UDP. Cada protocolo possui características adequadas para diferentes situações. Essa diferença é importante para a Cibersegurança, pois compreender TCP, UDP, portas e tráfego de rede será fundamental para estudos futuros de análise de redes e segurança.

💡 O que mudou no meu entendimento

Antes: eu associava TCP a "seguro/confiável" e UDP a "inseguro".

Depois: entendi que confiabilidade de transmissão não é a mesma coisa que segurança. TCP possui mecanismos para garantir a comunicação, mas isso não significa que ele seja, por si só, um protocolo de segurança.

# Miniguia de Estudos
Com base no conteúdo estudado, organizei os principais conceitos em uma sequência progressiva.

1. Fundamentos
- Redes de computadores
- Dispositivos de rede
- Cliente e servidor
- LAN e WAN
- Pacotes
- Protocolos
2. Modelos de rede
- Modelo OSI
- Modelo TCP/IP
- Encapsulamento
- Camadas de comunicação
3. Endereçamento
- IPv4
- IPv6
- Máscara de rede
- CIDR
- Sub-redes
- Gateway
- Endereços públicos e privados
4. Protocolos
- Ethernet
- ARP
- IP
- ICMP
- TCP
- UDP
- DNS
- DHCP
- HTTP
- HTTPS
- SSH
5. Infraestrutura
- Switch
- Roteador
- Roteamento
- NAT
- VLAN
-  Firewall
- VPN
6. Análise de redes
- Wireshark
- Nma
- Ping
- Traceroute
- Netstat / ss
- Nslookup / Dig
7. Próxima etapa: Cibersegurança
Depois de consolidar os fundamentos de redes, os próximos assuntos que pretendo estudar são:
- Segurança de redes;
- Monitoramento de tráfego;
- Firewalls;
- IDS/IPS;
- Vulnerabilidades de protocolos;
- Segurança Web;
- Pentest;
- Blue Team;
- SOC.
# Conclusão
O desenvolvimento deste projeto permitiu organizar o estudo de Redes de Computadores de forma estruturada, utilizando fontes de pesquisa e Inteligência Artificial como ferramentas de apoio à aprendizagem.

Durante o processo, foi possível compreender que o conhecimento de redes constitui uma base importante para entender como computadores, servidores, aplicações e outros dispositivos se comunicam.

Além do conhecimento técnico, o projeto também possibilitou desenvolver uma metodologia de estudo baseada em curadoria de fontes, elaboração de prompts, análise das respostas e identificação das próprias dificuldades.

Este projeto representa o início de uma trilha de estudos que pretendo continuar desenvolvendo, utilizando Redes de Computadores como base para posteriormente aprofundar meus conhecimentos em Segurança Computacional e Cibersegurança.


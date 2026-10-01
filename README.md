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
https://www.cisco.com/c/pt_br/solutions/small-business/resource-center/networking/networking-basics.html#~access-points
https://www.rfc-editor.org/rfc/rfc9293.pdf
https://www.rfc-editor.org/info/rfc768/
https://www.rfc-editor.org/info/rfc8200/
https://youtu.be/3b_TAYtzuho?si=q4qm-O2sn20EscXU
https://www.youtube.com/watch?v=2QGgEk20RXM&list=PLBbU9-SUUCwUyqvfypPAHWOaDr7Wz4P6t
https://www.youtube.com/watch?v=kP1kktlbUTs&pp=ygUPZ2xhdWtvIGNhcnZhbGhv

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

**Resposta**
### **Trilha de Estudos Progressiva em Redes de Computadores para Cibersegurança**

---

#### **Etapa 1: Fundamentos de Comunicação, Dispositivos e Mídias Físicas**

* **Assuntos a estudar:**
  * **Conceito de Rede e Protocolo:** Compreensão da comunicação como a troca de mensagens digitais regida por protocolos — conjuntos de regras pré-determinadas que garantem a padronização e a interoperabilidade entre equipamentos de diferentes fabricantes[1].
  * **Dispositivos da Infraestrutura:** Funções dos **Switches** (controladores de tráfego na rede local/LAN), **Roteadores** (encaminhadores de pacotes entre redes distintas e conexão à Internet) e **Access Points** (extensores e amplificadores da rede sem fio)[6].
  * **Meios Físicos e Sinalização:** Tipos de mídia de transmissão (cabos de cobre/par trançado, fibra óptica e ondas de rádio no ar/vácuo) e a conversão de dados em sinais elétricos, luminosos ou de rádio[11][12].
  * **Endereçamento Físico e Acesso ao Meio:** O papel da Placa de Rede (NIC), o **Endereço MAC** (identificador físico gravado pelo fabricante), o quadro Ethernet e o mecanismo de controle de acesso ao meio **CSMA/CD**[13][14].
* **Por que esta etapa é importante para a próxima?** Compreender como os bits são fisicamente transmitidos e organizados em quadros Ethernet dentro de uma rede local (LAN) fornece a base estrutural para entender como mensagens maiores são empacotadas e trafegam entre redes geograficamente separadas nas camadas superiores[11][13].

---

#### **Etapa 2: Arquitetura de Redes, Modelos de Referência e Encapsulamento**

* **Assuntos a estudar:**
  * **Modelos de Referência:** Estrutura e comparação entre o **Modelo OSI** (modelo conceitual de 7 camadas da ISO: Física, Enlace, Rede, Transporte, Sessão, Apresentação e Aplicação) e o **Modelo TCP/IP** (modelo prático de 4 camadas: Acesso à Rede, Internet, Transporte e Aplicação)[15].
  * **Unidades de Dados do Protocolo (PDU):** Identificação dos nomes dos dados em cada nível (Dados na Aplicação, Segmento/Datagrama no Transporte, Pacote na Rede, Quadro no Enlace e Bits na Camada Física)[15].
  * **Encapsulamento e Desencapsulamento:** Processo de adição de cabeçalhos de controle ao descer a pilha de protocolos na origem e a remoção desses cabeçalhos ao subir a pilha no destino[15].
  * **Diagnóstico por Camadas:** Uso da pilha de protocolos para resolução de problemas de forma estruturada (por exemplo, testando conectividade de camada 3 via ICMP/Ping antes de analisar falhas de camada de aplicação)[20].
* **Por que esta etapa é importante para a próxima?** Os modelos de referência fornecem o mapa mental do fluxo de dados. Sem dominar a divisão de responsabilidades entre as camadas e o conceito de encapsulamento, é impossível compreender o papel dos protocolos de roteamento e de transporte, ou analisar o tráfego de rede[21][29].

---

#### **Etapa 3: Camada de Rede (IP, IPv4, IPv6, Roteamento e ARP)**

* **Assuntos a estudar:**
  * **Endereçamento Lógico IPv4 e DHCP:** Estrutura do endereço IPv4, segmentação de rede (unicast, broadcast e multicast) e atribuição dinâmica de configurações de IP aos hosts via **DHCP**[30].
  * **Resolução de Endereços com ARP:** Funcionamento do **ARP (Address Resolution Protocol)** para descobrir o endereço MAC de destino associado a um IP na mesma rede local[36].
  * **Roteamento Inter-redes:** Encaminhamento de pacotes entre redes distintas por roteadores, uso de tabelas de roteamento e determinação do melhor caminho utilizando protocolos como OSPF, BGP e IS-IS[8].
  * **Protocolo IPv6 (RFC 8200):** Expansão do espaço de endereçamento para 128 bits, cabeçalho fixo simplificado (40 octetos), MTU mínimo de 1280 octetos, eliminação da fragmentação em roteadores intermediários (realizada apenas pela origem) e suporte a **Cabeçalhos de Extensão** (*Extension Headers*)[42].
* **Por que esta etapa é importante para a próxima?** A camada de rede garante a entrega de pacotes fim a fim entre hosts geograficamente distantes[31][32]. Compreender os cabeçalhos IP e a mecânica de roteamento é um pré-requisito essencial para estudar os protocolos da camada de transporte, que dependem do IP para estabelecer conexões confiáveis ou enviar datagramas[47].

---

#### **Etapa 4: Camada de Transporte (TCP vs. UDP e Mecanismos de Estado)**

* **Assuntos a estudar:**
  * **Endereçamento por Portas e Multiplexação:** Uso de números de porta (origem e destino) para identificar aplicações/serviços e multiplexar fluxos de dados (divisão em portas conhecidas, registradas e dinâmicas)[39].
  * **User Datagram Protocol — UDP (RFC 768):** Protocolo sem conexão (*connectionless*), leve, rápido, não confiável, sem garantia de ordem e com cabeçalho de apenas 8 bytes[47].
  * **Transmission Control Protocol — TCP (RFC 9293):** Protocolo orientado a conexão, confiável e fornecedor de fluxo de bytes ordenado[48].
  * **Mecanismos do TCP:**
    * **Estabelecimento e Encerramento de Conexão:** Handshake de 3 vias (`SYN`, `SYN-ACK`, `ACK`) para sincronização e encerramento em 4 etapas (`FIN`, `ACK`)[57].
    * **Máquina de Estados do TCP:** Estados da conexão (`LISTEN`, `SYN-SENT`, `SYN-RECEIVED`, `ESTABLISHED`, `FIN-WAIT`, `TIME-WAIT`, etc.)[65].
    * **Confiabilidade e Controle de Fluxo:** Números de sequência, confirmações acumulativas (`ACK`), técnica da Janela Deslizante, algoritmo de Nagle e prevenção da *Silly Window Syndrome* (SWS)[68].
* **Por que esta etapa é importante para a próxima?** A camada de transporte faz a ponte entre a infraestrutura de rede e os programas do usuário[51][75]. Entender como o TCP gerencia estados, conexões e fluxos de dados é indispensável para compreender o funcionamento das aplicações e analisar como atacantes exploram as fragilidades dessas sessões[76][77].

---

#### **Etapa 5: Camada de Aplicação e Serviços de Rede Básicos**

* **Assuntos a estudar:**
  * **Modelo Cliente-Servidor:** Funcionamento de aplicações onde clientes requisitam serviços e servidores os proveem, incluindo os conceitos de upload e download[39].
  * **DNS (Domain Name System - Porta UDP/TCP 53):** Sistema responsável por traduzir nomes de domínio legíveis por humanos em endereços IP numéricos e vice-versa[33].
  * **HTTP / HTTPS (Portas TCP 80 e 443):** Transferência de páginas hipertexto e recursos web entre navegadores e servidores[52].
  * **FTP (File Transfer Protocol - Portas TCP 20 e 21):** Transferência de arquivos utilizando portas separadas para controle e dados[33].
  * **Correio Eletrônico:** Funcionamento dos protocolos SMTP (envio - Porta TCP 25), POP3 e IMAP (recuperação/leitura de mensagens - Porta TCP 110)[33].
* **Por que esta etapa é importante para a próxima?** A camada de aplicação representa a interface direta com o usuário e com os sistemas de negócios[78][84]. Conhecer o funcionamento normal desses serviços permite identificar comportamentos anômalos e entender a superfície de ataque exposta na rede[77][89].

---

#### **Etapa 6: Segurança de Redes — Vulnerabilidades, Ataques e Defesas de Protocolo**

* **Assuntos a estudar:**
  1. **Ameaças e Vulnerabilidades Mapeadas nos Protocolos:**
    * **Camada de Rede (IP / IPv6):**
      * *Escuta Passiva (Eavesdropping):* Observação do conteúdo de pacotes por elementos no caminho da rede[89].
      * *IP Spoofing:* Falsificação do endereço de origem para injetar pacotes ou personificar hosts confiáveis[89].
      * *Reconhecimento (Varreduras):* Mapeamento de redes; no IPv6, a dimensão do espaço de endereçamento dificulta varreduras exaustivas[89].
      * *Ataques com Extension Headers e Fragmentação:* Manipulação de cabeçalhos de extensão no IPv6 para burlar controles ou desestabilizar sistemas com fragmentos sobrepostos[89][90].
    * **Camada de Transporte (TCP - RFC 9293):**
      * *Ataque de SYN Flooding:* Envio massivo de solicitações `SYN` com IPs falsificados para esgotar a memória do servidor (estruturas TCB) e causar negação de serviço[77].
      * *Ataques de Injeção Cega de Dados e Resets Cegos (Blind Reset Attacks):* Injeção de segmentos `RST` ou dados falsificados ao tentar adivinhar números de sequência válidos dentro da janela ativa[91].
      * *Previsibilidade do Número de Sequência Inicial (ISN):* Adivinhação de ISNs por atacantes fora da rota (*off-path*) para falsificar conexões[76][95].
      * *Fingerprinting do Sistema Operacional:* Análise passiva de opções do cabeçalho TCP, tempos de resposta e comportamento de janelas para identificar o SO da vítima[96].
  2. **Mecanismos de Defesa Integrados nas Especificações dos Protocolos:**
    * **Geração Criptográfica de ISN:** Uso de função pseudoaleatória (PRF) baseada em chave secreta e hash criptográfico para tornar o ISN imprevisível contra *off-path spoofing*[97][98].
    * **Mitigação com Challenge ACKs (RFC 5961):** Emissão de confirmações de desafio antes de abortar conexões estabelecidas ao receber pacotes `RST` ou `SYN` fora da sequência exata[91].
    * **Regra de Descarte de Fragmentos Sobrepostos (IPv6 - RFC 8200):** Exigência de que, se qualquer fragmento de um datagrama IPv6 for identificado como sobreposto, todo o datagrama deve ser silenciosamente descartado[90][100].
    * **Criptografia e Autenticação de Tráfego:**
      * *IPsec (AH e ESP):* Provê autenticação, integridade e confidencialidade diretamente na camada IP[42].
      * *TCP-AO (TCP Authentication Option):* Proteção de conexões TCP contra falsificação e injeção de dados[101][102].
      * *TLS e SSH:* Criptografia aplicável nas camadas superiores para proteger fluxos de dados confidenciais[89][103].
    * **Dispositivos de Borda:** Utilização de Firewalls com estado (*stateful firewalls*), VPNs e proxies para inspecionar pacotes e mitigar ataques DoS/DDoS[8].

# Cicatrizes do aprendizado
# Miniguia de Estudos
# Conclusão

# Conceitos Básicos de Redes

## O que é a Internet?
A **Internet** é formada por redes interconectadas que utilizam **protocolos comuns** para comunicação entre dispositivos.

---

## Tipos de Redes

| Tipo de Rede | Descrição |
|--------------|----------|
| **Rede Doméstica (Pequena)** | Conecta poucos dispositivos (ex: dispositivos pessoais em casa). |
| **SOHO (Small Office/Home Office)** | Conecta escritórios domésticos ou remotos a redes corporativas. |
| **Redes de Médio e Grande Porte** | Usadas por escolas, empresas e instituições maiores. |

---

## Tipos de Dados Pessoais

1. **Dados Voluntários**: Informações compartilhadas diretamente pelo usuário (ex: perfil de redes sociais).
2. **Dados Observados**: Dados coletados a partir das ações do usuário (ex: localização de celular).
3. **Dados Inferidos**: Informações geradas através da análise dos dados voluntários e observados (ex: sugestões de conteúdo no TikTok).

---

## Métodos de Transmissão de Sinais

- **Sinais Elétricos**: Utilizam fios de cobre para transmitir pulsos elétricos.
- **Sinais Ópticos**: Utilizam luz transmitida por fibra óptica.
- **Sinais Sem Fio**: Usam ondas de rádio, infravermelho, micro-ondas, etc.

---

## Definições Importantes

| Termo | Descrição |
|-------|-----------|
| **Largura de Banda** | Capacidade de uma rede para enviar dados, medida em Kbps, Mbps ou Gbps. |
| **Taxa de Transferência** | Quantidade real de dados transmitidos. |
| **Latência** | O tempo de viagem dos dados de um ponto a outro na rede. |

---

## O que é um Host?

Um **host** é qualquer dispositivo conectado a uma rede, capaz de enviar e receber dados. Ele pode ser: como cliente, servidor ou ambos.

---

## O que é uma Rede Ponto-a-Ponto (P2P)?

Em uma rede **Ponto-a-Ponto (P2P)**, todos os dispositivos são iguais e podem atuar tanto como **clientes** quanto **servidores**.

### Exemplos de Uso:
- **Compartilhamento de arquivos**: Como no caso do BitTorrent, onde arquivos são compartilhados diretamente entre os usuários.
- **Redes de comunicação**: Aplicações como Skype ou WhatsApp utilizam comunicação P2P para chamadas diretas.

---

# Infraestrutura de Rede

Este documento oferece uma visão geral detalhada sobre a infraestrutura de rede, seus componentes principais, protocolos e endereçamento. Ele explica conceitos fundamentais de comunicação em redes de computadores, como endereços IP, modelos de rede, e protocolos de comunicação.

---

## O que é Infraestrutura de Rede?

A **infraestrutura de rede** é a base física e lógica que permite a comunicação entre dispositivos, garantindo estabilidade e segurança. Ela é composta por:

### Componentes Principais:
- **Dispositivos Finais**: Equipamentos usados diretamente pelas pessoas (ex: computadores, impressoras).
- **Dispositivos Intermediários**: Equipamentos que conectam os dispositivos finais (ex: switches, roteadores).
- **Meios Físicos de Rede**: Caminhos pelos quais os dados trafegam (ex: cabos de rede, fibra óptica, sinais sem fio).

---

## Como os Protocolos Garantem a Comunicação na Rede?

Os **protocolos de rede** são regras que definem como os dispositivos se comunicam, garantindo que a troca de dados seja clara e organizada. Alguns componentes importantes dos protocolos são:

- Formato e tamanho da mensagem.
- Codificação.
- Temporização.
- Encapsulamento.
- Padrão de mensagens (solicitação/resposta).

---

## O que são Padrões de Rede?

**Padrões de rede** são regras e convenções que garantem que todos os dispositivos na rede "falem a mesma língua".

---

### 🌐 Modelo TCP/IP (4 camadas)

| Camada               | Descrição                                        | Exemplo de Protocolos               |
|----------------------|--------------------------------------------------|-------------------------------------|
| **Aplicação**         | Lida com dados do usuário e serviços (ex: HTTP)  | HTTP, FTP, DNS                     |
| **Transporte**        | Gerencia a comunicação entre dispositivos        | TCP, UDP                           |
| **Internet**          | Define roteamento e endereçamento de pacotes    | IP                                  |
| **Acesso à Rede**     | Gerencia o hardware físico e meios de transmissão | Ethernet, Wi-Fi                    |

---

### 🔽 Modelo OSI (7 camadas)

| Camada               | Descrição                                        | Exemplo de Protocolos               |
|----------------------|--------------------------------------------------|-------------------------------------|
| **Aplicação**         | Onde os programas do usuário interagem com a rede | HTTP, FTP, DNS                     |
| **Apresentação**      | Formata os dados (ex: compressão, criptografia)  | SSL/TLS                            |
| **Sessão**            | Gerencia a comunicação entre aplicativos        | RPC, NetBIOS                       |
| **Transporte**        | Assegura a entrega completa e ordenada dos dados | TCP, UDP                           |
| **Rede**              | Roteamento e endereçamento de dados             | IP                                  |
| **Enlace de Dados**   | Garante a entrega confiável na mesma rede       | Ethernet, PPP                      |
| **Física**            | Transmite os bits através de cabos ou sinais    | Cabos, fibras ópticas, Wi-Fi        |

---

## Tabela de Comparação


| Camada OSI            | Camada TCP/IP          |
|-----------------------|------------------------|
| **7. Aplicação**       | **Aplicação**           |
| **6. Apresentação**    | **Aplicação**           |
| **5. Sessão**          | **Aplicação**           |
| **4. Transporte**      | **Transporte**          |
| **3. Rede**            | **Internet**            |
| **2. Enlace de Dados** | **Acesso à Rede**       |
| **1. Física**          | **Acesso à Rede**       |

---

## O que é Encapsulamento?

**Encapsulamento** é quando os dados são "empacotados" com informações extras em cada camada da rede para garantir que cheguem ao destino de forma correta e organizada. Esse processo permite que os computadores entendam quem enviou, quem deve receber e o que deve ser feito com a mensagem.

---

## O que é um Quadro Ethernet?

Um **quadro Ethernet** O quadro Ethernet é o envelope padrão usado dentro das redes locais (como em casa ou na empresa). Ele contém:

- **Endereço MAC de Destino**: Quem recebe os dados.
- **Endereço MAC de Origem**: Quem enviou os dados.
- **Preamble**: Sincroniza a comunicação.
- **Tamanho e Tipo de Mensagem**: Define o conteúdo e formato dos dados.
- **Verificação de Erro**: Garantia de que os dados não foram corrompidos.

---

## O que é um Endereço IPv4?

O **IPv4** é o endereço digital **único de cada dispositivo em uma rede**, usado para garantir que os dados cheguem ao destino certo. Ele está associado à placa de rede (NIC) do dispositivo.

**IPv4** é um endereço de 32 bits, dividido em 4 blocos de 8 bits (octetos), cada um representado por um número de 0 a 255. Exemplo de formato: 

| **Rede** | **Rede** | **Rede** | **Host** |
|----------|----------|----------|----------|
| 192      | 168      | 5        | 11       |


### Tipos de Comunicação IPv4

| Tipo      | Descrição                                                            | Exemplo                                         |
|-----------|----------------------------------------------------------------------|-------------------------------------------------|
| **Unicast** | (1 -> 1):  Um único dispositivo de origem e destino.      | Acesso a um site na web.                       |
| **Broadcast** | (1 -> Todos):  Um dispositivo envia dados para todos os dispositivos da rede local ao mesmo tempo. | Pedido de IP via DHCP.                         |
| **Multicast** | (1 -> grupo): Um dispositivo envia dados apenas para um grupo específico de dispositivos interessados.      | Uma live de vídeo transmitida apenas para quem entrou no evento. |

---

## Endereço Público vs Privado

| Tipo de Endereço | Descrição                                                                 | Exemplo                     |
|------------------|---------------------------------------------------------------------------|-----------------------------|
| **Público**      | Visível na internet, utilizado para identificar dispositivos globalmente. | Endereço IP do Google       |
| **Privado**      | Usado em redes internas, requer NAT para comunicação com a internet.      | 192.168.0.1 (rede local)    |

### Faixas de Endereços Privados:
- **Classe A**: 10.0.0.0 a 10.255.255.255
- **Classe B**: 172.16.0.0 a 172.31.255.255
- **Classe C**: 192.168.0.0 a 192.168.255.255

---

## Loopback e APIPA

| Tipo              | Descrição                                                              | Exemplo                           |
|-------------------|------------------------------------------------------------------------|-----------------------------------|
| **Loopback**      | Endereço para testar a própria máquina (localhost).                    | 127.0.0.1                         |
| **APIPA**         | Atribuído quando o DHCP não está disponível, permitindo comunicação local. | 169.254.x.x                       |

---

## O que é um Endereço IPv6?

O **IPv6** é a versão mais recente do protocolo de endereçamento, com 128 bits, substituindo o IPv4 para suportar o número crescente de dispositivos na Internet. Ele é representado por 8 grupos de 4 caracteres hexadecimais (que podem usar letras de A a F). Exemplo: 2001:0db8:85a3:0000:0000:8a2e:0370:7334


### Regras para Simplificar Endereços IPv6

| Regra                       | Descrição                              | Exemplo                               |
|-----------------------------|----------------------------------------|---------------------------------------|
| **Remover Zeros à Esquerda** | Elimina zeros à esquerda de cada grupo. | 01AB → 1AB                           |
| **Usar "::" para Blocos de Zeros** | Representa blocos de zeros consecutivos. | 2001:0db8:0000:0000:0000:0000:abcd:1234 → 2001:db8::abcd:1234 |

🚨 **Atenção**: O "::" só pode ser usado uma vez no endereço.

---

## Transição IPv4 para IPv6

- **Pilha Dupla**: Dispositivos utilizam IPv4 e IPv6 juntos.
- **Encapsulamento**: IPv6 encapsulado dentro de pacotes IPv4 para atravessar redes antigas.
- **Tradução (NAT64)**: Converte pacotes IPv6 ↔ IPv4 para compatibilidade.

---

## IP Estático vs IP Dinâmico

| Tipo de IP   | Descrição                                          | Exemplo                             |
|--------------|----------------------------------------------------|-------------------------------------|
| **Estático** | O IP é configurado manualmente.                    | 192.168.0.100                       |
| **Dinâmico** | O IP é atribuído automaticamente pelo DHCP.        | Atribuição automática via DHCP      |

---

## Como Funciona o DHCP?

| Etapa        | Descrição                                                            |
|--------------|----------------------------------------------------------------------|
| **Descoberta** | O dispositivo pede um IP.                                           |
| **Oferta**     | O servidor sugere um IP.                                            |
| **Solicitação**| O dispositivo aceita o IP.                                          |
| **Confirmação**| O servidor confirma e atribui o IP.                                  |

🎯 **Tudo isso acontece em segundos!**

---

## O que é o Gateway (porta de saída)?

| Definição                                        |
|--------------------------------------------------|
| Um **gateway** é uma "porta de saída" que faz a comunicação entre duas redes diferentes. Ele encaminha os dados do seu dispositivo para fora da sua rede local e também recebe os dados de fora, trazendo-os de volta para o seu dispositivo. |

Exemplo: Quando você digita "www.google.com", a solicitação sai do seu computador, vai para o **gateway** (geralmente o roteador) e, de lá, é direcionada para a internet.

---

## O que é NAT (Network Address Translation) e sua Importância?

| Definição                                        |
|--------------------------------------------------|
| **NAT** é um processo feito pelo roteador que converte os endereços IP privados da rede local em um único IP público para se comunicar com a internet. Isso permite que vários dispositivos usem a mesma conexão sem precisar de IPs públicos exclusivos. |

---

## O que é Endereço MAC e Endereço IP?

| Tipo de Endereço | Definição                                                   | Exemplo         |
|------------------|-------------------------------------------------------------|-----------------|
| **Endereço IP**  | Identifica um dispositivo dentro de uma rede (lógico).     | 192.168.0.10    |
| **Endereço MAC** | Identifica de forma única o dispositivo (físico).          | 00:1A:2B:3C:4D:5E |

---

## Como Descobrir o Endereço MAC de um IP?

| Etapa do Processo                  | Descrição                                                             |
|------------------------------------|-----------------------------------------------------------------------|
| **ARP**                            | O **ARP** (Address Resolution Protocol) é um protocolo que mapeia um IP para um endereço MAC. |
| **Processo**                       | 1. Computador envia um broadcast para toda a rede, perguntando: "Quem tem o IP X?" |
|                                    | 2. Dispositivo com o IP correspondente responde com seu endereço MAC. |
|                                    | 3. Computador armazena a informação na tabela ARP para uso futuro.   |

---

## Quando o IP Está em Outra Rede?

| Situação                                  | Descrição                                                            |
|------------------------------------------|----------------------------------------------------------------------|
| **Destino na mesma rede**                | O pacote de dados vai diretamente ao destino dentro da mesma rede.    |
| **Destino em outra rede**                | O pacote vai primeiro para o **gateway** (roteador) para ser encaminhado à rede correta. |

---

## O que o Roteador Faz Exatamente?

| Passo                               | Descrição                                                             |
|-------------------------------------|-----------------------------------------------------------------------|
| **Recebe o pacote de dados**        | O roteador recebe o pacote e lê o IP de destino.                      |
| **Consulta a tabela de roteamento** | O roteador consulta sua tabela de roteamento (GPS da rede).           |
| **Decide o próximo salto**          | O roteador decide para qual porta enviar o pacote.                    |
| **Coloca o endereço MAC**           | O roteador coloca o endereço MAC correto no pacote.                   |
| **Envia o pacote**                  | O pacote é enviado ao próximo roteador ou ao destino final.           |

---

## Como o Roteador Sabe para Onde Mandar?

| Tipo de Tabela de Roteamento | Descrição |
|------------------------------|-----------|
| **Tabela Manual**             | Configurada manualmente por um técnico. |
| **Tabela Automática**         | Aprendizada dinâmico, onde o roteador aprende os caminhos por onde os dados devem passar. |

---

## TCP vs UDP

| Protocolo | Características                                       | Ideal para                                                |
|-----------|--------------------------------------------------------|-----------------------------------------------------------|
| **TCP**   | Confiável, divide dados em segmentos numerados, com confirmação de recebimento. | Websites (HTTPS/HTTP), e-mails (SMTP/IMAP/POP3), FTP.    |
| **UDP**   | Mais rápido, sem confirmação de recebimento, e perda de pacotes tolerável. | Vídeo ao vivo, jogos online, chamadas VoIP.               |

---

## Números de Porta: Como os Serviços São Identificados

| Serviço         | Porta           |
|-----------------|-----------------|
| **Web (HTTP)**  | Porta 80        |
| **Web segura (HTTPS)** | Porta 443  |
| **E-mails (SMTP)** | Porta 25      |
| **FTP**          | Porta 21        |
| **DNS**          | Porta 53        |
| **IMAP**         | Porta 143       |
| **POP3**         | Porta 110       |
| **SSH**          | Porta 22        |
| **Telnet**       | Porta 23        |
| **TFTP**         | Porta 69        |
| **NTP**          | Porta 123       |

---

## Cliente e Servidor

| Tipo         | Descrição                                                              |
|--------------|------------------------------------------------------------------------|
| **Servidor** | Computador ou programa que fornece serviços/informações pela internet (ex: servidor web). |
| **Cliente**  | Computador ou programa que solicita essas informações (ex: navegador). |

---

## URL e URI

| Tipo de Identificador | Descrição                                               | Exemplo                         |
|-----------------------|---------------------------------------------------------|---------------------------------|
| **URI**               | Endereço na internet que aponta para um recurso.       | https://meusite.com/pagina.html |
| **URL**               | Endereço exato de um recurso.                           | https://meusite.com/pagina.html |
| **URN**               | Identifica um recurso sem dizer onde está.             | urn:isbn:0451450523             |

---

## DNS (Sistema de Nomes de Domínio)

| Definição                                        | Porta |
|--------------------------------------------------|-------|
| O **DNS** traduz nomes de sites (ex: www.google.com) para endereços IP, permitindo que os computadores encontrem os sites na internet. | 53 (TCP/UDP) |


## Clientes e Servidores Web

| Elemento        | Descrição                                                                 |
|-----------------|---------------------------------------------------------------------------|
| **Navegador (Cliente)** | O navegador (como Chrome, Firefox, etc.) é o **cliente** que faz solicitações ao servidor web para carregar sites. |
| **Servidor Web** | O servidor web é o computador ou programa que hospeda as páginas web e responde às solicitações feitas pelos navegadores. |
| **Portas**       | O navegador acessa o servidor web nas portas **80 (HTTP)** para conexões não seguras e **443 (HTTPS)** para conexões seguras (criptografadas). |
| **HTTPS**        | **HTTPS** é a versão segura do HTTP, que usa criptografia para proteger os dados trocados entre o cliente e o servidor. |
| **HTML**         | **HTML** (HyperText Markup Language) é a linguagem usada para definir a estrutura e o conteúdo das páginas web, incluindo texto, imagens, links e outros elementos. |

---

## FTP (File Transfer Protocol)

| Função        | Descrição                                              | Porta |
|---------------|--------------------------------------------------------|-------|
| **FTP**       | Protocolo para enviar e receber arquivos via rede.     | 21 (controle), 20 (transferência) |

---

## Telnet e SSH

| Protocolo | Descrição                                        | Porta |
|-----------|--------------------------------------------------|-------|
| **Telnet**| Acesso remoto sem segurança.                    | 23    |
| **SSH**   | Acesso remoto seguro com criptografia. Sempre prefira SSH. | 22    |

---

## E-mails

| Protocolo | Descrição                                                  | Porta |
|-----------|------------------------------------------------------------|-------|
| **SMTP**  | Envia e-mails                                              | 25    |
| **POP3**  | Baixa e-mails (sem manter no servidor)                     | 110   |
| **IMAP**  | Lê e-mails no servidor (mais moderno)                      | 143   |

---

## Mensagens e Chamadas

| Tipo de Comunicação  | Protocolo                    | Porta (Comum) |
|----------------------|------------------------------|---------------|
| **Mensagens**        | Usam protocolos próprios para troca em tempo real. | Variável (Ex: XMPP - 5222, WhatsApp - 5222) |
| **Chamadas de voz/vídeo** | Usam VoIP para transformar voz em dados e trafegar pela internet. | 5060 (SIP - Session Initiation Protocol), 1935 (RTMP para vídeo) |

---


## Comandos Úteis

| Comando              | Descrição                                           |
|----------------------|-----------------------------------------------------|
| **ipconfig**         | Exibe informações básicas da rede (IP, gateway).   |
| **ipconfig /all**    | Exibe informações detalhadas, incluindo DNS e MAC. |
| **ipconfig /release**| Libera o endereço IP atual (caso use DHCP).        |
| **ipconfig /renew**  | Solicita um novo endereço IP ao servidor.          |
| **ping**             | Testa a conectividade com outro computador/site.   |
| **netstat**          | Mostra quais portas estão em uso, e com quais endereços IP o computador está se comunicando..                  |
| **tracert**          | Mostra o caminho entre seu computador e o destino, passando por todos os roteadores no meio do caminho.. |
| **nslookup**         | Descobre o IP de um site ou verifica DNS está funcionando.          |

---

## Conclusão

Este material apresenta **conceitos básicos de rede**, com foco em protocolos, endereçamento IP, modelos de rede e comunicação, que são fundamentais para o entendimento de como as redes funcionam no dia a dia.

O resumo foi **criado por mim** com base nos conteúdos do **Cisco Networking Academy**, que oferece uma introdução completa aos princípios de redes, abordando tanto os fundamentos teóricos quanto práticos. O objetivo aqui foi organizar esses conceitos de maneira clara e acessível, facilitando o aprendizado e a aplicação desses conhecimentos no contexto de redes de computadores.

---

**Fontes**: 
- Cisco Networking Academy
- Documentação técnica e recursos online sobre redes

**Autora**: Biatriz Gomes



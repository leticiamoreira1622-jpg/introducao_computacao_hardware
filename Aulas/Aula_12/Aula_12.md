# Aula 12 #
# Aula 12 – Internet: História, Conceitos, Protocolos e Navegadores

## Objetivo
Compreender a origem e evolução da Internet, seus conceitos fundamentais, principais protocolos de comunicação e o papel dos navegadores.

## Estrutura da Entrega
Cada grupo deve incluir neste repositório:

### 1. História da Internet
# A Evolução da Internet: Do Militar ao Comercial

## 1.1. O Pontapé Inicial: ARPANET (Décadas de 1960/1970)
Nascida em plena Guerra Fria e financiada pelo Departamento de Defesa dos EUA (através da ARPA), a **ARPANET** foi a grande precursora da internet moderna.

* **O Objetivo:** Criar uma rede de comunicação descentralizada que resistisse a falhas catastróficas (como um ataque militar). Se um nó da rede caísse, os dados encontrariam outro caminho.
* **O Marco (1969):** A primeira mensagem foi enviada entre a UCLA e a Universidade de Stanford. A ideia era digitar "LOGIN", mas o sistema caiu após as duas primeiras letras (**"LO"**).
* **A Tecnologia:** Introduziu a **comutação de pacotes**, base para o envio de dados que usamos até hoje.

## 1.2. Expansão Acadêmica e Militar (Décadas de 1970/1980)
A rede cresceu e começou a conectar o conhecimento global, deixando de ser um projeto puramente militar.

* **A Padronização (1983):** Adoção do protocolo **TCP/IP**. Esse "idioma universal" permitiu que redes de computadores totalmente diferentes conversassem entre si.
* **A Divisão:** O segmento militar se separou (MILNET), e a rede principal expandiu-se rapidamente por universidades e centros de pesquisa nos EUA e na Europa, popularizando o uso de e-mails acadêmicos e transferência de arquivos (FTP).

## 1.3. A Criação da WWW por Tim Berners-Lee (1989/1990)
Até aqui, a internet era puramente textual e complexa. Tudo mudou no CERN (Organização Europeia para a Pesquisa Nuclear).

* **A Sacada:** O cientista britânico **Tim Berners-Lee** percebeu a dificuldade em compartilhar informações entre pesquisadores e inventou a **World Wide Web (WWW)**.
* **As Ferramentas:** Ele desenvolveu o sistema de hiperlinks (onde um clique te leva a outra página), a linguagem **HTML** e o protocolo **HTTP**.
* **Diferenciação Importante:** A *Internet* é a infraestrutura física (os cabos e computadores conectados); a *Web* é a forma de navegar e visualizar as páginas de maneira amigável.

## 1.4. Comercialização e Popularização (Anos 1990)
Nos anos 90, o governo americano retirou as restrições ao uso comercial, abrindo as portas para o mundo.

* **Os Navegadores:** O surgimento de browsers gráficos como o **Mosaic** e o **Netscape** transformou a rede em algo visual, com imagens, cores e cliques.
* **O Boom Econômico:** Foi a era da *Web 1.0*. Surgiram gigantes como Yahoo!, Amazon, eBay e, em 1998, o Google. 
* **O Cotidiano:** A internet discada entrou nas casas das pessoas, transformando a rede mundial de computadores em um fenômeno de massa e mudando a sociedade para sempre.

### 2. Conceitos Fundamentais
#### 2.1. Internet vs. Web (A Diferença Crucial)
Embora usados como sinônimos no dia a dia, são conceitos completamente diferentes:

* **Internet:** É a **infraestrutura física** global. Trata-se da rede de redes de computadores conectada por cabos submarinos, satélites, roteadores e fibra óptica. Pense na internet como o **sistema de rodovias** mundial.
* **Web (World Wide Web):** É apenas **um dos serviços** que roda em cima dessa infraestrutura. É o sistema de páginas interconectadas por hiperlinks que acessamos via navegador. Pense na Web como os **carros e caminhões** que viajam pelas rodovias da internet.
* *Outros serviços da internet que não são a Web:* E-mail (protocolo IMAP/SMTP), chamadas de voz e vídeo (VoIP), jogos online, aplicativos de mensagens (WhatsApp) e transferências de arquivos (FTP).

#### 2.2. Arquitetura Cliente-Servidor
É o modelo de design de rede que dita como a informação é distribuída na internet. O processo funciona em um ciclo básico de **Requisição e Resposta**:<br>

I.  **O Cliente:** É o dispositivo ou aplicativo que solicita informações. Exemplos: seu navegador (Chrome, Safari), o app do Instagram no seu celular ou sua Smart TV. Ele inicia o contato fazendo uma **requisição** (request).<br>
II.  **A Rede:** A requisição viaja pela internet.<br>
III.  **O Servidor:** É um computador de alta performance, projetado para ficar ligado 24/7, que armazena os dados, sites e sistemas. Ele processa a requisição do cliente e envia de volta uma **resposta** (response) contendo os dados solicitados (como o código HTML de um site ou uma imagem).<br>


#### C. Endereços IP (Internet Protocol)
O endereço IP é a **identidade única** de cada dispositivo conectado à rede. Ele funciona exatamente como o endereço postal da sua casa, garantindo que os dados cheguem ao destino correto.

##### Exemplos Práticos de Uso:

* **IPv4 (O formato clássico):** Composto por quatro blocos de números de 0 a 255, separados por pontos.
    * *Exemplo:* `192.168.1.1` (comum para o roteador da sua casa) ou `172.217.22.14` (um dos IPs do Google).
* **O "GPS" dos Pacotes de Dados:** Quando você digita `www.google.com`, seu navegador usa um sistema (chamado DNS) para traduzir esse nome no IP real do servidor do Google. O seu computador (ex: IP `192.168.1.50`) envia uma mensagem dizendo: *"Por favor, envie o site do Google para o IP 192.168.1.50"*.
* **IP Público vs. IP Privado:** * Sua smart TV, seu celular e seu computador possuem **IPs Privados** diferentes dentro da sua casa para o roteador saber quem é quem.
    * Para o resto do mundo lá fora, o seu roteador usa um único **IP Público** (fornecido pela sua operadora de internet) para representar toda a sua casa.

### 3. Protocolos

Os protocolos são as regras e combinados que os computadores usam para conversar entre si. Sem eles, as máquinas enviariam dados em formatos incompatíveis, tornando a comunicação impossível.

#### 3.1. TCP/IP (O Protocolo de Base)
O **TCP/IP** não é apenas um protocolo, mas um conjunto (pilha) de protocolos que formam a espinha dorsal da internet. Ele controla como os dados são divididos, endereçados, enviados e recebidos.

* **Função:** * O **IP (Internet Protocol)** cuida do endereçamento e da rota, garantindo que os dados saibam de onde saíram e para onde vão.
    * O **TCP (Transmission Control Protocol)** garante que a entrega seja confiável. Ele quebra o arquivo em pequenos pedaços (pacotes), verifica se algum se perdeu no caminho e os organiza na ordem correta ao chegar no destino.
* **Exemplo Prático:** Quando você baixa um arquivo pesado ou assiste a um vídeo por streaming. Se um pacote de dados do arquivo "sumir" no caminho por causa de uma oscilação na rede, o TCP percebe a falha e pede para o servidor reenviar apenas aquele pedacinho perdido, garantindo que o arquivo não fique corrompido.

#### 3.2. HTTP / HTTPS (O Protocolo da Web)
O **HTTP (Hypertext Transfer Protocol)** e sua versão segura, o **HTTPS**, são os protocolos utilizados para transferir os dados das páginas que navegamos.

* **Função:** Estabelecer a comunicação entre o seu navegador (cliente) e o servidor que hospeda um site. O HTTPS adiciona uma camada de criptografia (geralmente usando SSL/TLS), garantindo que os dados trafegados entre o seu dispositivo e o servidor sejam ilegíveis para terceiros que tentem interceptá-los.
* **Exemplo Prático:** * Ao ler um artigo de notícias em um site comum antigo: **HTTP**.
    * Ao digitar sua senha no internet banking ou inserir os dados do cartão de crédito em uma loja virtual: **HTTPS** (identificado pelo ícone de cadeado na barra de endereços do navegador).

#### 3.3. DNS (Domain Name System)
O **DNS** funciona como a "lista de contatos" da internet. Como computadores só entendem números (endereços IP) e humanos lembram mais facilmente de nomes, o DNS faz o meio de campo.

* **Função:** Traduzir nomes de domínios amigáveis em endereços IP reais.
* **Exemplo Prático:** Quando você digita `www.wikipedia.org` no seu navegador, a primeira coisa que o seu computador faz (em milissegundos) é perguntar para um Servidor DNS: *"Ei, qual é o número IP da Wikipedia?"*. O DNS responde algo como `198.35.26.96`, e aí sim o seu navegador consegue se conectar ao servidor do site.

#### 3.4. FTP (File Transfer Protocol)
O **FTP (File Transfer Protocol)** é um dos protocolos mais antigos da internet, criado especificamente para a movimentação de arquivos.

* **Função:** Permitir a transferência de arquivos (upload e download) entre um cliente e um servidor de forma rápida e direta, sem a necessidade de passar por uma interface web complexa.
* **Exemplo Prático:** Um programador que acabou de criar um site no seu computador pessoal e precisa enviar todos os códigos, imagens e vídeos do projeto para a empresa de hospedagem onde o site vai ficar publicado no ar. Para isso, ele usa um programa de FTP (como o FileZilla) para "jogar" os arquivos diretamente na pasta do servidor remoto.

### 4. Navegadores
Os navegadores são os softwares que funcionam como a "janela" do usuário para a Web. A principal função deles é traduzir linhas de código complexas em uma interface visual, interativa e amigável.

#### 4.1. A Interpretação de HTML, CSS e JavaScript
Quando você acessa um site, o servidor envia um pacote de arquivos de texto puro contendo três tecnologias essenciais. O navegador atua como um "tradutor" que processa esses arquivos simultaneamente:

* **HTML (HyperText Markup Language):** É o **esqueleto** da página. O navegador lê o HTML para entender a estrutura e o conteúdo do site (onde há um parágrafo, um título, uma imagem ou um formulário).
* **CSS (Cascading Style Sheets):** É a **estética** (a roupa) do site. O navegador interpreta o CSS para aplicar as cores, fontes, alinhamentos, espaçamentos e layouts sobre o esqueleto do HTML.
* **JavaScript (JS):** É o **comportamento** (os músculos) da página. É uma linguagem de programação executada diretamente no navegador do usuário. Ela permite que a página seja dinâmica — atualizando conteúdos em tempo real, exibindo animações, validando formulários ou reagindo a cliques sem precisar recarregar o site inteiro.

#### 4.2. Principais Motores de Renderização (Browsers Engines)
O "coração" de qualquer navegador é o seu **motor de renderização** (ou *layout engine*). Trata-se do componente interno do software responsável por pegar o código (HTML/CSS) e desenhar fisicamente os pixels na tela do usuário. 

Embora existam dezenas de navegadores diferentes no mercado, a grande maioria deles utiliza um dos três motores principais abaixo:

##### I. Blink
* **Navegadores que utilizam:** Google Chrome, Microsoft Edge, Opera, Brave e Vivaldi.
* **Origem:** Criado pela Google em 2013 como uma ramificação (*fork*) do WebKit. Hoje, é o motor mais dominante do mercado mundial.

##### II. Gecko
* **Navegadores que utilizam:** Mozilla Firefox (e suas variantes focadas em privacidade, como o Tor Browser).
* **Origem:** Desenvolvido pela Mozilla Foundation. É conhecido por ser um motor de código aberto altamente independente e focado em manter a Web aberta e competitiva, sem o monopólio de uma única empresa.

##### III. WebKit
* **Navegadores que utilizam:** Apple Safari (no macOS, iOS e iPadOS).
* **Origem:** Desenvolvido pela Apple (baseado inicialmente em um projeto de código aberto chamado KHTML). 
* *Curiosidade:* Devido às regras da App Store da Apple, até muito recentemente, *todos* os navegadores que rodam no iPhone (incluindo o Chrome e o Firefox para iOS) eram obrigados por contrato a usar o motor WebKit por baixo dos panos, funcionando essencialmente como "capas" visuais sobre a engine do Safari.

### 5. Exercício Prático – Análise de Protocolos
<img width="1919" height="983" alt="Captura de tela 2026-05-04 154132" src="https://github.com/user-attachments/assets/9374e486-bf6d-47f2-969d-ab91b668dffc" />
<img width="1919" height="948" alt="Captura de tela 2026-05-04 154452" src="https://github.com/user-attachments/assets/d33244ec-17fb-4ada-a5be-1d27e4f7bbc0" />

## Organização dos Arquivos
- Criar uma pasta com o nome do grupo (ex.: `Grupo1_Protocolos`, `Grupo2_Navegadores`).
- Dentro da pasta, incluir:
  - `historia_internet.pdf` ou `historia_internet.md`
  - `conceitos.pdf` ou `conceitos.md`
  - `protocolos.pdf` ou `protocolos.md`
  - `navegadores.pdf` ou `navegadores.md`
  - `analise_protocolos.pdf` ou `analise_protocolos.png`
  - `README.md` com breve descrição do trabalho.

## Critérios de Avaliação
- Clareza e organização das explicações.
- Correção conceitual na análise dos protocolos.
- Exemplos práticos bem escolhidos.
- Participação de todos os integrantes.

## Reflexão Individual
Cada integrante deve produzir um texto curto (1 página) respondendo:  
**“Qual protocolo você considera mais essencial para o funcionamento da Internet e por quê?”**<br>
Se a gente tivesse que escolher o protocolo que sustenta o planeta inteiro nas costas, o prêmio vai direto para o **IP (Internet Protocol)**, jogando em dupla com o **TCP**. Sem eles, a internet simplesmente vira um monte de computador isolado e sem utilidade. <br>

A internet nada mais é do que uma colcha de retalhos de bilhões de redes diferentes (a da sua casa, a do Google, a de uma universidade no Japão). O IP é o idioma universal que faz todas essas máquinas conversarem. A sacada genial aqui é que ele não envia arquivos inteiros de uma vez; ele quebra tudo (suas fotos, áudios, sites) em "pacotinhos", carimba o endereço de destino e joga na rede.<br>

Cada pacote pode seguir um caminho totalmente diferente pelo mundo — um vai por cabo submarino, outro por satélite. Se um cabo romper no meio do caminho, os pacotes mudam de rota sozinhos. É aí que o TCP entra como o "gerente de qualidade": ele confere se tudo chegou direitinho no destino, pede para retransmitir o que sumiu e junta as peças na ordem certa.<br>

O mais legal é que o IP não quer saber *o que* está carregando. Ele entrega um vídeo da Netflix com o mesmo carinho que entrega uma mensagem do WhatsApp ou uma página de texto. O DNS é incrível porque nos poupa de decorar números e o HTTP faz a Web ser bonita, mas o TCP/IP é o motor que mantém o mundo conectado de verdade. Sem ele, não tem nem rede para os outros protocolos rodarem.<br>




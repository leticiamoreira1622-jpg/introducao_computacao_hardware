# Aula 12 #
Abra um navegador (Chrome, Edge ou Firefox).
Pressione F12 para abrir as ferramentas de desenvolvedor.
Vá até a aba Network (Rede).
Acesse um site qualquer (ex.: https://www.ufrn.br).
Observe as requisições (Requests) que aparecem na lista.
Clique em uma delas para ver detalhes.
Identifique:
Request → O que o navegador pediu (ex.: arquivo HTML, imagem, CSS).
Response → O que o servidor enviou de volta.
Status Code → Exemplo:
200 OK → Sucesso.
404 Not Found → Página não encontrada.
301 Moved Permanently → Redirecionamento.
Registre os resultados em um documento ou slide.
🔹 Opção 2: Usando o Wireshark
Instale e abra o Wireshark.
Selecione a interface de rede ativa (Wi-Fi ou Ethernet).
Clique em Start Capture para iniciar a captura de pacotes.
Acesse um site simples (ex.: https://www.google.com).
No Wireshark, filtre os pacotes usando:
http → para ver requisições HTTP.
dns → para ver consultas de nomes.
Identifique:
Request → Pacote enviado pelo cliente (ex.: GET /index.html).
Response → Pacote recebido do servidor (ex.: HTTP/1.1 200 OK).
Status Code → Indicado na resposta HTTP.
Salve a captura ou faça um print da tela para incluir no relatório.
🔹 Entregável
Cada grupo deve produzir um relatório ou slides com:
Um exemplo de Request.
Um exemplo de Response.
O Status Code analisado.
Publicar o material no GitHub da disciplina na pasta da Aula 12.

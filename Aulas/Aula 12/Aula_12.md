# Aula 12 #
Abra um navegador (Chrome, Edge ou Firefox). <br>
Pressione F12 para abrir as ferramentas de desenvolvedor. <br>
Vá até a aba Network (Rede). <br>
Acesse um site qualquer (ex.: https://www.ufrn.br). <br>
Observe as requisições (Requests) que aparecem na lista. <br>
Clique em uma delas para ver detalhes.<br>
Identifique:<br>
Request → O que o navegador pediu (ex.: arquivo HTML, imagem, CSS).<br>
Response → O que o servidor enviou de volta.<br>
Status Code → Exemplo:<br>
200 OK → Sucesso.<br>
404 Not Found → Página não encontrada.<br>
301 Moved Permanently → Redirecionamento.<br>
Registre os resultados em um documento ou slide.<br>
🔹 Opção 2: Usando o Wireshark<br>
Instale e abra o Wireshark.<br>
Selecione a interface de rede ativa (Wi-Fi ou Ethernet).<br>
Clique em Start Capture para iniciar a captura de pacotes.<br>
Acesse um site simples (ex.: https://www.google.com).<br>
No Wireshark, filtre os pacotes usando:<br>
http → para ver requisições HTTP.<br>
dns → para ver consultas de nomes.<br>
Identifique:<br>
Request → Pacote enviado pelo cliente (ex.: GET /index.html).<br>
Response → Pacote recebido do servidor (ex.: HTTP/1.1 200 OK).<br>
Status Code → Indicado na resposta HTTP.<br>
Salve a captura ou faça um print da tela para incluir no relatório.<br>
🔹 Entregável<br>
Cada grupo deve produzir um relatório ou slides com:<br>
Um exemplo de Request.<br>
Um exemplo de Response.<br>
O Status Code analisado.<br>
Publicar o material no GitHub da disciplina na pasta da Aula 12.<br>
<img width="1919" height="983" alt="Captura de tela 2026-05-04 154132" src="https://github.com/user-attachments/assets/9374e486-bf6d-47f2-969d-ab91b668dffc" />
<img width="1919" height="948" alt="Captura de tela 2026-05-04 154452" src="https://github.com/user-attachments/assets/d33244ec-17fb-4ada-a5be-1d27e4f7bbc0" />



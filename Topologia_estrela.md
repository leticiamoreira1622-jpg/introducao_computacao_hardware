# Topologias, Dispositivos e Meios
## Estrela
Topologia comum em redes modernas em que todos os dispositivos encontram-se conectados a um ponto central. <br>
### **Conceito** <br>
A comunicação entre dois hosts obrigatoriamente realiza passagem pelo nó central de forma que, se houver a quebra de um cabo de computador, apenas esse fica fora da rede. <br>
### **Dispositivo Central** <br>
Switch (inteligente) ou um Hub (Obsoleto) <br>
### **Hosts Conectados** <br>
Agem de maneira independente, o desempenho da rede é dependente da capacidadede processamento do dispositivo central. <br>
<img width="2048" height="2048" alt="image" src="https://github.com/user-attachments/assets/8ce0cd50-e52b-4e2b-acda-3eba32494bd0" />
## Barramento
Utilizada antigamente com cabos coaxiais, comum em barramento internos de placas-mãe. <br>
### **Conceito** <br>
Os hosts compartilham o mesmo meio físico *(backbone)*, a informação é enviada a todos, mas apenas o destinatário realiza o processamento. <br>
### **Dispositivo Central** <br>
O dispositivo central é inexistente, porém existem *terminadores* na extremidade para evitar que o sinal reflita e causa interferência. <br>
### **Hosts conectados** <br>
Disputam o mesmo espaço de fala, se o cabo principal sofre corte, a rede inteira para de funcionar. <br>
<img width="2048" height="2048" alt="image" src="https://github.com/user-attachments/assets/6983c816-1cc0-4e82-ba6f-6ec0e0345b4e" />
## Anel (Ring) 
### **Conceito** <br>
Os dados viajam de maneira unidirecional, cada host recebe a mensagem e a repassa para o próximo até chegar ao destino. <br>
### **Dispositivo Central** <br>
Não há dispositivo central lógico, embora em implementações físicas (*Token Ring*), se use um concentrador chamado MAU (Multistation Access Unit).
### **Hosts Conectados** <br>
Funcionam como repetidores de sinal, o ponto fraco é que, se um único host falhar, o anel é quebrado e a comunicação é interrompida.
<img width="3999" height="2283" alt="image" src="https://github.com/user-attachments/assets/ea0da188-7e38-4950-90b4-630921947beb" />
## Malha (Mesh)
Modelo da redundância total. Cada dispositivo pode estar conectado a vários outros. <br>
### **Conceito** <br>
Existem múltiplos caminhos para a informação chegar ao destino de modo que, se uma rota congestionar, o dado segue por outra. <br>
### **Dispositivo Central** <br>
O dispositivo central é inexistente. <br>
### **Hosts conectados** <br>
Possuem várias interfaces de conexão. É a topologia base da Internet e das Redes Mesh Wi-Fi modernas, garantindo que a rede nunca caia completamente. <br>
<img width="2048" height="2048" alt="image" src="https://github.com/user-attachments/assets/fc778e86-2736-48f0-b0a2-faecca8196f7" />

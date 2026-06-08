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
## Tabela comparativa
| | Função principal | Vantagens | Limitações | Exemplo |
| --- | --- | --- | --- | --- |
| **Hub** | Interconexão de computadores em uma rede local, não identifica o destinatário e, portanto, replica a informação para todas as portas | Extremamente barato e simples para uso | Gerador de muito tráfego desnecessários, colisão de dados e insegurança, uma vez que qualquer um na rede pode acessar o que os outros recebem. | Hub são raros atualmente, presentes apenas em museus de tecnologia e laboratórios específicos para análise de tráfego básico. |
| **Switch** | Conexão de dispositivos em uma rede local (LAN) de maneira inteligente, armazena o endereço físico (MAC Address) de cada aparelho conectado a ele. | A entrega de informação é exclusiva ao destinatário, o que aumenta a velocidade e a segurança | Impossibilidade de conetar redes diferentes, apenas gerenciamento da conversa interna. | A rede de uma empresa, em que dezenas de computadores e impressoras trocam arquivos rapidamente de forma eficiente. |
| **Roteador**| Escolha da melhor rota para os dados e interconexão de redes diferentes | Gerenciamento de endereços IP com farewall integrado que permite a tradução de endereços (NAT), possibilitando que vários aparelhos usem uma única conexão de internet. | Mais caro e complexo em relação à configuração. | Aparelho que a operadora instala em residências (roteador + switch + antena Wi-fi).|
## Classificação
### **Meios Guiados**
**Par Trançado** <br>
Comum em redes locais (LANs). Pares de fio de cobre entrelaçados para redução de interferência eletromagnética. <br>
**Cabo Coaxial** <br>
Condutor central de cobre cercado por material isolante e uma malha metálica, resistente a interferência. <br>
**Fibra Óptica** <br>
Transmissão de dados através de pulsos de luz em fios de plástico ou plástico, rápido e imune a interferências elétricas.
### **Meios Não Guiados** 
**Wi-fi** <br>
Utiliza-se de radiofrequência para conexão de dispositivos em uma área local. <br>
**Bluetooth** <br>
Tecnologia de curto alcance com enfoque na conexão de periféricos e dispositivos pessoais (PAN). <br>
**Satélite** <br>
Utiliza-se de micro-ondas para cobrir distâncias globais, ideal para locais remotos. <br>
**Infravermelho** <br>
Requer linha de visão de visão direta e curto alcance. <br>
Aqui está a tabela convertida para o formato Markdown:

| Meio | Velocidade | Distância Máxima | Custo | Sensível a Interferência? |
| :--- | :--- | :--- | :--- | :--- |
| **Par Trançado** | Alta (até 10Gbps) | ~100 metros | Baixo | Sim |
| **Fibra Óptica** | Altíssima (Tbps) | Quilômetros | Alto | Não |
| **Wi-Fi** | Média/Alta | ~50 metros | Médio | Sim (paredes, outros sinais) |
| **Satélite** | Média | Global | Muito Alto | Sim (clima/nuvens) |

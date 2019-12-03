# Switches and Hubs

## Hub
O Hub é como se fosse um T elétrico, todo sinal que ele recebe ele envia para todas as portas (inclusive de volta para a porta que enviou)

Implementa apenas a camada 1 - A camada física

## Switches

Além da camada 1, eles implementam:

- Camada 2 - O processo de Enlace ( Controle de fluxo, de erros, enquadramento e acesso ao meio. )

- Camada 3 - Switch Router - A camada de rede ( Endereçamento IP )

- Camada 4 - Switch de aplicação - Além da camada de rede, interpreta o tipo de protocolo ( diferenciar se é um arquivo, uma página web, etc). Permite separar a banda, ex: 15% para WEB, 20% para FTP, etc.

### Tabela SAT

Dentro do Switch, existe uma _Search Address Table_, que fica salva na RAM, e conforme recebe os dados da conexão salva os dados de quem está conectado em qual porta.

O Preenchimento dos endereços se dá através do envio de endereço de origem.

A quantidade de conexões depende da arquitetura de conexão do switch e dos dispositivos conectados (barramento, etc), e também do sistema operacional.

### Domínio de Colisão
- Hub: 1 Domínio de colisão, quando tem um problemas todas máquinas são afetadas.
- Switch: Não acontece colisão, pois colisão só acontece quando o meio é compartilhado.

### Domínio de Broadcast
- Hub: 1 Domínio
- Switch: 1 Domínio também, pois switch não filtra pacote broadcast, compartilha para todos.
- Roteados (Ou um switch de camada 3): Cada porta é uma rede diferente, separando os domínios broadcast.

## Problemas da camada 2
- Muito broadcast sobrecarrega o switch
- MAC é um endereço plano, não tem hierarquia

## Switch camada 3
- Camada 3 faz roteamento, é capaz de dividir a rede em redes menores. Um equipamento de uma rede só fala com equipamentos de sua rede - a não ser que seja roteado pelo roteador para um equipamento de outra rede.
- Mesma funcionalidade de um roteador, mas adequado para LANs

## Protocolo IEE 802.1D Spanning Tree
- Soluciona os loops de rede: Deixa o caminho menos eficiente em stand-by, e ativa ele só quando há um problema com os outros caminhos.

### Métodos de comutação
- Cut-through: Passa de uma porta para a outra apenas lendo o endereço, sem verificar a integridade (os erros). Os erros são verificados apenas no equipamento destino.
- Store-and-forward: Recebe os dados, armazena, verifica a integridade de quadro em quadro, e se estiver OK, passa o pacote adiante.
- Adaptative cut-through: Funciona de ambas as formas, dependendo da sua configuração.

### Capacidade do Backplane
(Backplane = barramento do switch)

Baseado em um switch de 24 portas 1GB:
- Blocking: Velocidade menor que 24 Gbps
- Non-blocking: Velocidade igual a 24 Gbps

### Link Resiliente
Igual ao spanning tree, mas a escolha do caminho menos eficiente é manual

### Link Agregation
Comunicação entre switches

### Espelhamento de tráfego
Toda tráfego do switch é encarregado para a porta que tem o espelhamento, e neste porta pode se conectar um sniffer que sabe de todo tráfego da rede.

### Virtual LAN (VLAN)
Virtual Local Network: Fazer uma rede local via software

## Características a serem consideradas na escolha dos switches

# Qual switch mais adequado para cenário 1:
Catalyst 2960-L ( $502.99 )
Small and medium-sized businesses
Simple device management
Layer 2

# Quais switches mais adequados para cenário 2:
Catalyst 3850-24XS
Switch camada 4

Cisco Catalyst 6880
Switch camada 3

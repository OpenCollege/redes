# Redes Remotas

O ADSL é assimétrico, e seu foco é domestico, pois o consumidor doméstico faz mais downloads do que uploads.

## Principais tipos de serviços
- Acesso a Internet
  - xDSL
  - Cabo

- Conexão entre LANs:
 - Frame Relay
 - MPLS
 - Ethernet Metropolitana
 - ATM
 - Link Privativo

- Backbone
  - SDH / Sonet

## SDH / Sonet
`SDH` - Padrão Americano   
`Sonet` - Padrão Europeu

Servem para fazer multiplexação de: Fibra ótica ou rádio microondas.  
Esta tecnologia pode ser utilizada também em rádio de altíssima frequência.   
É uma capacidade muito alta, por isso não é vendido para empresas.

## Link Privativo / Link Dedicado
Basicamente puxar um cabo de uma ponta a outra para fazer a comunicação.
Geralmente chamado de um serviço `transparente`, por não passar pelo backbone.

`Nuvem` não é link dedicado. Nuvem passa pelo backbone da empresa e lá ele é transmitido misturado a outras transmissões.

Desvantagens:  
O custo é alto para manter o equipamento sempre disponível.
O preço aumenta conforme a distância aumenta e conforme mais velocidade se necessita.

Vantagens:
Não vai ter problema de congestionamento

Quando é ideal:  
Quando se há necessidade de tráfego constante; durante a maior parte do dia.

## MPLS
Utiliza o TCP/IP.  
O TCP/IP transporta pacotes baseado no IP de origem e IP destino. O serviço MPLS, no entanto, há algumas características adicionais que aumentam o desempenho. Ao invés do encaminhamento ser através do endereço IP, cada pacote possui um rótulo, que diz a rota aonde o pacote deve ir.

Vantagens:  
- Quality of Service ( QoS ) : Graças ao IPv6
- Segurança

Vantagens em relação a um link dedicado:  
- Se conecta direto com a operadora, não precisa passar pelo ponto central
- Custo menor pois a conexão com operadora é mais curta

## Ethernet
Utilizada em:
- Link dedicado
- Nuvem

## SD-WAN (Software Defined)

## ATM
Camada Física - Camada ATM - Camada AAL  

ATM - Camada de rede da arquitetura TCP/IP. Faz a comunicação via circuitos.  

É o ideal, muitas vezes inclusive é utilizado no backbone das operadoras.  

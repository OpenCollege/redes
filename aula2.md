# Redes de computadores

## Hardware - Tecnologia de transmissão
- Broadcast
- Ponto a ponto

# Protocolo TCP/IP
- Aplicação
- Transporte
- Rede
- Enlace
- Física

QUEM IMPLEMENTA
Enlace e física: Placa de rede   
Aplicação, transporte e rede: Sistema Operacional  

## Física
Transforma dados em sinais e realiza transmissão
Implementada na placa de rede

## Enlace
Enquadramento, controle de fluxo, acesso ao meio, controle de erros (serve para verificar integridade)

PROTOCOLOS
- LAN: Protocolo Ethernet
- WLAN: Protocolo 802.11 (wi-fi)
- WAN: HDLC, PPP

## Rede
Responsável pelo roteamento

PROTOCOLOS
- IP
- ICMP

## Transporte
- `Multiplexação dos dados`: Divide os dados em pacotes menores
- `Endereçamento de aplicações`
- `Confiabilidade`: Verifica se houve perda de pacotes na Rede
Verifica se recebeu pacotes duplicados
- `Controle de fluxo`
- `Controle de congestionamento`

PROTOCOLOS

- `TCP`: Mais confiável
- `UDP`: Mais rápido
Dados que são armazenados (ex: Vídeos da internet), geralmente se usa TCP, pois é importante a qualidade.
Dados que não são armazenados (ex: Video-chamadas, jogos), geralmente se usa UDP

## Aplicação
Realiza a comunicação entre processo cliente e processo servidor
> Não existe servidor, é processo servidor e processo cliente

PROTOCOLOS
- FTP
- SMTP
- HTTP
- DNS
- IMAP
- POP

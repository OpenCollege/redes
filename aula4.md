# Modulação, Multiplexação e Comutação

# Modulação do Sinal
MoDem = Modulation | Demodulation
A modulação transforma dados digitais (ou qualquer outro tipo de dado) em sinal analógico.


![img](assets/aula4-91fa4.png)
1. Bits
2. Modulação por amplitude ( ASK )
3. Modulação por frequência ( FSK )
4. Modulação por fase ( PSK )
5. Modulação por amplitude de quadratura de onda ( QAM ) - Mais utilizada hoje

## Modulação em Quadratura

União de amplitude e fase
QAM - Geral sinal analógico e gera também sinal digital.
-É a única técnica que serve tanto para modulação quanto para codificação

# Codificação

Converte Dado Digital em Sinal Digital.
Serve para adaptar, para que o sinal possa ser transmitido mais longe, mesmo que não mude o tipo de sinal.

## Técnicas de Codificação
Monofase:
- `NRZ-L` (Não retorno ao 0)
- `NRZ-I` (Não retorno ao 0 invertido)
Bifase:
- `Manchester` (Utilizada na primeira ethernet)
- `Manchester Diferencial`
Especiais:
- `PCM` Pulse Code Modulation
- `DM`

### NRZ
- O reconhecimento é reconhecimento no início da transmissão do bit.
- Quanto tem perda de sincronização, geralmente se perde o início, ou seja, a identificação do bit.

### Bifase
- Reconhecimento do bit no meio da transmissão
- Evita perda de sincronização

### PCM
Geralmente não é classificada junto com as técnicas de codificação, é considerada uma técnica especial por converter dados analógicos em sinais digitais.
- Utiliza um codificador (Codec)
Etapas:
1. Amostragem
2. Quantização
3. Codificação

### Resumindo
Os sinais digitais sofrem mais atenuação que os sinais analógico, pois os sinais digitais tem uma amplitude menor.
É preciso converter o sinal para que ele possa ser transmitido em uma distância maior, utilizando modulação de sinal, codificação, ou pcm.

# Multiplexação

Serve para dividir um canal em mais canais para ter transmissões simultâneas.
Divide um canal físico em canais lógicos.

## Por frequência (FDM)
Aloca frequências menores para diferentes canais

Ex: ADSL - Assimetric, downstream channel is bigger ( 1 de voz, 1 downstream, 1 upstream )
ADSL Divide em 3 canais por frequência e depois divide por tempo.

## Por fatias de tempo (TDM)
Aloca o canal inteiro (com todas frequências) por um determinado tempo para transmissões individuais.

- `Síncrona` Uma fatia de tempo é alocada ao dispositivo, tendo ou não dados para ser transmitidos. Pode gerar ociosidade de transmissão no canal.
- `Assíncrona/Estatística` Quando o computador não tem nada a transmitir, passa para o próximo. Não gera ociosidade.

Ex: Rede Local

## Por tamanho da onda de luz (WDM)
Separa pelo comprimento de onda (cor). Utilizado na fibra ótica.


# Comutação

Definir a reserva de recursos na rede na hora da transmissão dos dados; Aloca recursos para a transmissão.

### `Circuito`
Se tem congestionamento, não fecha o circuito. Depois de fechado não ocorre congestionamento durante a transmissão. Ex: Telefonia convencional
Não há perda de pacotes. Pacotes chegam ordenados.

Etapas:
1. Estabelecimento de conexão
2. Transferência de dados
3. Encerramento de conexão

### `Pacote`
Tipo cartas do Sedex. Talvez chegue, ordem não é mantida, etc.
- Podem não seguir a mesma rota.
- Podem ser perdidos
- Não chegam em ordem

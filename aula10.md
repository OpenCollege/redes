# Enlaçe em Redes Locais

### `MAC`
- Controle de Erros
- Enquadramento
- Acesso ao meio

### `LLC`
- Controle de fluxo

O LLC é opcional. Inicialmente só se tinha Broadcast, no qual não precisa ser feito controle de fluxo, então apenas a camada MAC era o suficiente. Hoje, como a maioria dos pacotes são encaminhados através de switchs, precisa do LCC para fazer o controle de fluxo.

## Topologias

#### `Em estrela`

Ex: Switches, hubs.

Caso o elemento central falhe, a rede para. O Hub é uma tomada T, ele recebe os dados e repassa, sem nenhum filtro. O Switch tem o endereço origem e o endereço destino, portanto ele encaminha para a porta correta.

#### `Em anel`

Ex: Token

Não tem colisão de pacotes, pois o token faz esse tipo de controle.

#### `Em barra`

Ex: Broadcast

Fica ouvindo a rede, se não tem nada para transmitir, transmite os dados. Caso duas estações transmitam ao mesmo tempo, há a colisão de pacotes.

#### `Mistas`

Mais de uma das anteriores ao mesmo tempo.

## Formas de codificação de linha

## Formas de acesso ao meio

## CSMA / CD
- Não é utilizado em full-duplex 

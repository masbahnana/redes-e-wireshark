---
share: true
---
### Formato de cabeçalho do TCP

![[Drawing 2023-06-16 14.34.33.excalidraw]]


É o TCP Header que contém as informações importantes que são necessárias para o segmento TCP corretamente ao destino. O TCP tem 20 bytes e contém os campos:

- **Source Por Address ou Porta de Origem:** identifica a porta que está sendo utilizada pelo processo de origem para enviar para o TCP. Ou seja é o campo que contém o endereço da porta do remetente.
- **Destination Port Address ou Porta de Destino:** identifica a porta usada pelo processo de destino para receber o segmento TCP. E essa é a porta do destinatário.
- **Sequence Number ou Número de sequência:** é usado para identificar a posição dos dados do segmento TCP em relação aos dados que foram antes enviados. É o número de bytes do primeiro byte de dados enviados em um pacote TCP. Quando a conexão é estabelecida pela 1º vez por meio de uma mensagem *SYN*, o número de sequência inicial *(ISN - Initial Sequence Number)* é definido. O *ISN* pode ser qualquer número de 0 a 4.294.967.295 e os dados reais começam em *ISN+1*.
- **Conhecimento ou Confirmação:** É onde o receptor confirma que recebeu os dados corretamente e é o próximo número de sequência esperado pelo remetente *ACK*.
- **HLEN**: significa *Header Length* ou *Tamanho do cabeçalho*, esse campo indica o tamanho ou comprimento do cabeçalho TCP em palavras de 4 bytes (ou 32 bits). O tamanho mínimo pode ser de 20 bytes e o máximo é de 60 bytes.
- **Reserved** **ou Reservado**: não muito usada pois foi incluída para uso futuro e deve ser definida como 0 quando o pacote TCP é enviado. Essa reserva permite que o TCP no futuro possa ter extensões e/ou melhorias, como ainda não tem nenhuma funcionalidade esse valor fica zerado.
- **Flags ou bandeiras ou sinalizadores**: que são utilizados para controlar o comportamento do TCP, como indicar se o segmento é uma solicitação de conexão *(SYN)*, uma confirmação *(ACK)* ou uma solicitação de encerramento *(FIN)*.


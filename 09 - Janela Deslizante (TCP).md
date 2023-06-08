---
share: true
---
### E a janela deslizante?

A *"window wize"* ou janela deslizante é um mecanismo utilizado pelo TCP que otimiza a transmissão de dados em uma rede. Nessa técnica o transmissor envia uma quantidade limitada de dados ao receptor e aguarda a confirmação *(ACK)* antes de enviar mais dados, assim evitando que o transmissor envie muitos dados que possam sobrecarregar a rede ou o receptor.

- A janela é implementada através de dois valores, o tamanho da janela e o valor de confirmação *(ACK)* que o receptor envia de volta;
- O tamanho da janela é o número máximo de bytes que o transmissor pode enviar sem esperar por uma confirmação;
- O valor de confirmação indica ao transmissor quantos bytes foram recebidos com sucesso pelo receptor.

Ou seja, a janela ajusta a quantidade de dados enviados conforme a capacidade da rede, recepção e do receptor, o que (de novo) garante eficiência, confiabilidade durante a transmissão.
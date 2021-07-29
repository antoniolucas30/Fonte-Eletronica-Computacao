# Projeto Fonte de Eletrônica

Nesse projeto, realizamos a esquematização de uma fonte que recebe como entrada uma corrente alternada de 127 V, entregando uma corrente contínua de 3 a 12 V com amperagem de 100 mA.

## Alunos

| Nome                                   | Número USP | Contato (Gmail)     |
|----------------------------------------|------------|---------------------
| Samuel Victorio Bernacci               | 12703455   | samubernacci@usp.br |   
| Antonio Lucas Sales Cavalcante Barbosa | 12677529   | antoniolucas@usp.br |   
| Gustavo Wadas Lopes                    | 12745640   | gustavowlopes@usp.br| 



## Componentes do Projeto

* Transformador: Componente que irá transformar a diferença de potencial vinda da tomada, que possui RMS (root mean square) de 179,6 V, para uma menor e mais próxima do objetivo da nossa fonte (por volta de 19 V no pico). O seu funcionamento se dá a partir de suas bobinas, as quais, possuintes de um campo magnético, reduzem a corrente à desejada.

* Diodos: São usados para retificar a corrente alternada vinda da tomada, usados na ponte de diodo que faz uma retificação de dupla onda que otimiza a voltagem da tomada através da inversão de um dos semicírculos da função da voltagem da tomada. 

* Capacitor: Armazena a carga durante os picos da corrente alternada, liberando corrente quando a tensão do capacitor é maior que a tensão da fonte. O capacitor foi escolhido para um ripple de 10%, calculando chegamos à um valor de 463 uF, foi escolhido o valor comercial próximo de 470 uF. 

* Diodo Zener: Regula a tensão máxima para 13 V, conduzindo apenas quando estiver acima dos 13 V e retém essa voltagem, regulando assim a tensão máxima. 

* Resistores: Limitam a corrente que passam pelos componentes para não exceder o limite destes. 

* Potenciômetro: Resistor variável utilizado para ajustar a tensão que vai para o transistor. 

* Transistor: Utilizado para limitar a passagem de corrente diretamente para a saída.



## Circuito do Falstad

<img src="https://i.imgur.com/OjdFo0b.png" alt="Circuito">
<a href="https://tinyurl.com/ye7d76mt">Circuito do Falstad</a>

## Circuito esquematizado e Placa PCB no Eagle

<img src="https://i.imgur.com/NZEK3ZQ.png"  alt="Circuito_Eagle">
<img src="https://i.imgur.com/nYqBlXP.png" alt="Placa_PCB">

## Tabela de peças, quantidades e valores

| Quantidade | Componente             | Valor                  |
| --- | ---------------------- | ---------------------- |
| 4   |  <a href="https://www.baudaeletronica.com.br/diodo-1n4004.html">Diodo 1N4004</a>          |  R$ 0,13 * 4 = R$ 0,52 |
| 1   | <a href="https://www.baudaeletronica.com.br/capacitor-eletrolitico-470uf-25v.html?gclid=Cj0KCQjwl_SHBhCQARIsAFIFRVVx7R6O5ASnN9eOsV4yikA8JqS3I0bVRsjiD1Ygu-r7GOdJRdqGlBgaAl4eEALw_wcB">Capacitor 470uF </a>        | R$ 0,45                |
| 2   | <a href="http://www.tiggercomp.com.br/novaloja/product_info.php?cPath=29&products_id=116">Resistor 1k ohms</a>       | R$ 0,13 * 2 = R$ 0,26                |
| 1   | <a href="http://www.tiggercomp.com.br/novaloja/product_info.php?cPath=29&products_id=132">Resistor 4,7k ohms</a>     | R$ 0,13                 |
| 1   | <a href="https://www.baudaeletronica.com.br/potenciometro-linear-de-10k-10000.html">Potênciometro 10k ohms</a> | R$ 1,79                |
| 1   | <a href="https://www.fazolocomponentes.com.br/_loja_/p/315661/diodo-zener-12w-13v-in-5243">Diodo Zener 1N5243</a>     | R$ 0,30                |
| 1   | <a href="https://www.baudaeletronica.com.br/transistor-npn-bc548.html">Transistor NPN - BC548</a> | R$ 0,19                |
| 1   | <a href="https://produto.mercadolivre.com.br/MLB-989896074-transformador-trafo-1818v-500ma-bivolt-eletronica-eletrica-_JM#position=34&search_layout=stack&type=item&tracking_id=83f121cf-e449-4516-b01e-541d4255aafb">Transformador 18V</a>        | R$ 34,99               |
| 1 | <a href = "https://www.baudaeletronica.com.br/led-de-alto-brilho-10mm-vermelho.html">LED 3 - 3,2 V</a> | R$ 0,70
 
 **Total:** R$ 39,38

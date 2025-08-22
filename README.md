# FundamentosSistemasCircuitVerse

O arquivo representa um circuito da aula de Fundamentos de Sistemas Computacionais do dia 20/08/2025 a ser aplicado no site circuitverse.org.

O exercício define como meta a necessidade de carregar em um ambiente GITHUB os arquivos necessários para o circuito, além de 5 cenários de teste.

Foram feitos os seguintes circuitos:
o	Somador ou Meio-Somador (6 bits)
o	Multiplexador (de 1 para 2 vias)
o	Comparador (1 bit e 6 bits)

Além desses, para melhor desenvolvimentos da matéria também foram feitos os seguintes circuitos:
o	Full Hadder (1 bit e 6 bits)
o	Or (1 bit e 6 bits)
o	ADD (1 bit e 6 bits)

Conforme as instruções do quadro apresentado pelo professor, foi um projeto dos circuitos (um processador), capaz de executar as operações, denominado de ULA.

Os sub-circuitos utilizados na ULA foram: Comparador, FullHadder, And, Or.

Entre a ULA e os multiplexadores foram colocadas saídas de teste para verificação dos resultados parciais de cada sub-circuito.

Os cenários de teste foram:
o	Todos os 6 bits ligados em A e B:
Entrada: 111111 111111
Saída:
    - (Sel1 = 0 ou 1) e (Sel2 = 1): 111111 (este é o que consta da figura)
    - (Sel1 = 1) e (Sel2 = 0): 111110 

o	Todos os 6 bits desligados em A e B:
Entrada: 000000 000000
Saída:
    - (Sel1 = 1) e (Sel2 = 0 ou 1): 000000
    - (Sel1 = 0) e (Sel2 = 1): 000000
    - (Sel1 = 0) e (Sel2 = 0): 111111

o	Os bits de A e B alternadamente ligados:
Entrada: 101010 010101
Saída:
    - (Sel1 = 1) e (Sel2 = 0 ou 1): 111111
    - (Sel1 = 0) e (Sel2 = 0 ou 1): 000000

o	Os 3 primeiros bits de A e os 3 últimos de B ligados:
Entrada: 111000 000111
Saída:
    - (Sel1 = 0) e (Sel2 = 0 ou 1): 000000
    - (Sel1 = 1) e (Sel2 = 0 ou 1): 111111

o	Os 3 primeiros bits de B e os 3 últimos de A ligados:
Entrada: 000111 111000
Saída:
    - (Sel1 = 0) e (Sel2 = 0 ou 1): 000000
    - (Sel1 = 1) e (Sel2 = 0 ou 1): 111111

![img](img/CircuitExercicio.png)

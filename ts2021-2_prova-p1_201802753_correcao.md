<div align=center>
  <img src="brasaooficialcolorido.png">
</div>

#### <p style="text-align: center;">Universidade Federal de Goiás</p>
#### <p style="text-align: center;">Instituto de Informática</p>
#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>
#### <p style="text-align: center;">Teste de Software - 2021/2</p>
#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>
####  <p style="text-align: center;"> Prova P1 - 16/02/2022</p>

Matrícula: 201802753
Nome: Amanda Lobo Gomes
<p><font color=green>Nota: 8.9</font></p>

1. Quanto ao objetivo do Teste de Software, responda as duas questões seguintes:
   1. (**0,5 ponto**) Qual o objetivo primário da atividade de teste de software?
   <br>
   R: Testes de software tem como objetivo primário revelar defeitos no software desenvolvido. <font color=green>Certo</font>
   <br>
   2. (**0,5 ponto**) O que acontece, quando não se atinge este objetivo primário?
   <br>
   R: Quando o teste não atinge seu objetivo primário, ou seja, encontrar defeitos no software, as chances de entregar um produto que não atende aos requisitos do cliente aumenta, aumentando a chance de desenvolver um produto de má qualidade. <font color=red>Errado</font>
   <br>
2. (**1,0 ponto**) Explique o que é o teste exaustivo e porque sua execução não é possível.
   <br>
   R: O teste exaustivo testa todas as entradas possíveis do código da aplicação. Geralmente, esse teste é inviável pois podem existir infinitas entradas possíveis do código. <font color=green>Certo</font>
   <br>
3. (**1,0 ponto**) Cite pelo menos duas limitações da Técnica de Teste Funcional e duas da Técnica de Teste Estrutural.
   <br>
   R: Teste funcionais dependem de uma boa especificação de requisitos, e não garantem que partes essenciais ou críticas do software sejam executadas. Os testes estruturais identificam caminhos de execução a partir da implementação do produto em teste. Assim, o número de caminhos pode ser infinito ou muito grande, pois a cada decisão dobra e cada looping multiplica. Outra desvantagem é que os caminhos presentes na especificação podem ser esquecidos na implementação. <font color=green>Certo</font>
   <br>
4. (**1,0 ponto**) Descreva pelo menos um dos quatro níveis de teste constantes da literatura especializada.
   <br>
   R: Os quatro níveis de teste constantes são: Testes de aceitação; Testes de sistema; Testes de integração; Testes unitários. Testes unitários verificam o comportamento das menores unidades da aplicação, por exemplo, uma classe ou um método em linguagem orientada a objetos. <font color=green>Certo</font>
   <br>
5. (**1.0 ponto**) Descreva qual o propósito do critério de teste funcional Particionamento por Classes de Equivlência.
   <br>
   R: O teste por particionamento por classes de equivalência divide o domínio de entrada do programa em classes de dados. Os dados de teste são derivados a partir das classes de equivalência. Primeiro, identifica-se as classes de equivalência. Depois, define-se os casos de teste. <font color=orange>Parcialmente correto. Nota 0,4</font>
   <br>
6. (**1.00 ponto**) Existe algum tipo de hierarquia em relação aos critérios de teste estrutural, todos os nós, todos os arcos e todos os caminhos? Se sim, explique-a, considerando a perspectiva dos níveis de cobertura desejados.
   <br>
   Sim existe uma hierarquia em relação aos critérios todos nós, todos arcos e todos caminhos. Dependendo do nível de cobertura desejado, como o nível 2, que atende ao critério todos os arcos, é obrigatoriamente necessário atender ao critério todos os nós. Para atingir o nível de cobertura 7, que atende ao critério todos os caminhos, é obrigatóriamente necessário atender aos níveis de cobertura anteriores, ou seja, atender aos critérios de todos os nós e todos os arcos. <font color=green>Certo</font>
   <br>
7. Considere a especificação, a seguir, de um hipotético programa que objtiva a classificação de um triângulo, a partir dos valores informados para os seus três lados.

   a) Dado um triângulo cujos segmentos medem A, B e C, que são números inteiros positivos na faixa de 0 a 100. Esse triângulo somente existirá se: (A + B < C) ou (A + C < B) ou (B + C < A).
   R: Considere as condições: (A + B > C) ou (A + C > B) ou (B + C > A)
   b) Quanto às medidas dos seus lados o triângulo, poderá ser classicado em:
         • Isósceles = quando possui dois lados com a mesma medida;
         • Escaleno = quando todos os seus lados têm medidas diferentes;
         • Equilátero = quando todos os lados tem a mesma medida;
         • Acutângulo = quando o quadrado de um dos seus lados é menor que a soma do quadrado dois outros dois. (A<sup>2</sup> < B<sup>2</sup> + C<sup>2</sup>).
         • Retângulo: quando o quadrado de um dos seus lados é igual à soma do quadrado dois outros dois. (A<sup>2</sup> = B<sup>2</sup> + C<sup>2</sup>).
         • Obtusângulo: quando o quadrado de um dos seus lados é maior que a soma do quadrado dois outros dois. A<sup>2</sup> > B<sup>2</sup> + C<sup>2</sup>.

7.1 (**2.0 pontos**) Definir uma tabela de decisão para o teste tanto da existência do triângulo, quanto para a definição do seu tipo. Consulte exemplo de tabela de decisão na tarefa 005.
|R1: A+B>C ou A+C>B ou B+C>A|F|V|V|V|V|V|V|V|V|
|---|---|---|---|---|---|---|---|---|---|
|R3: A=B||F|F|F|F|V|V|V|V|
|R4: B=C||F|F|V|V|F|F|V|V|
|R4: A=C||F|V|F|V|F|V|F|V|
|Não é um triângulo|X|||||||||
|Equilátero|||||||||X|
|Isóceles|||X|X||X||||
|Escaleno||X||||||||

<font color=green>Certo</font>

7.2 (**2.0 pontos**) Criar os conjunto de casos de teste necessários para a cobertura das combinações constantes da tabela de decisão, seguindo o seguinte padrão:
|CT|Lado A|Lado B|Lado C|Resultado|
|---|---|---|---|---|
|01|0|0|0|Não é um triângulo|
|02|2|5|6|Escaleno|
|03|5|3|5|Isóceles|
|04|5|3|3|Isóceles|
|05|2|2|1|Isóceles|
|06|7|7|7|Equilátero|

<font color=green>Certo</font>

INSTRUÇÕES:
1. Tipo: Prova individual;
2. Local de Entrega: Plataforma Turing
3. Forma de Entrega: Entregar este arquivo, editado com suas respostas, no formato .md, nominado da seguinte forma: ts2021-2_prova-p1_mat.md, onde mat deverá ser substituído pelo número da sua matrícula.
4. **Entrega diferente da especificada não será avaliada.**
5. Data da Entrega: 22/02/2022, as 23h59min.
6. Critério de Aceitação: arquivo entregue, conforme solicitado.

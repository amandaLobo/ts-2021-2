<div align=center>
  <img src="brasaooficialcolorido.png">
</div>

#### <p style="text-align: center;">Universidade Federal de Goiás</p>
#### <p style="text-align: center;">Instituto de Informática</p>
#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>
#### <p style="text-align: center;">Teste de Software - 2021/2</p>
#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>
####  <p style="text-align: center;"> Prova P2 - 12/04/2022</p>

Matrícula: 201802753

Nome: Amanda Lobo Gomes

<p><font color="red">Nota 3,5</font></p>


1. Quanto ao Processo de Teste de Software, responda as duas questões seguintes:
   1. (**0,5 ponto**) Defina os seguintes conceitos Processo de Teste de Software, Projeto de Teste de Software e Plano de Teste de Sofware.
   O Processo de Testes de Software consiste em uma estruturação de fases e artefatos que tem o objetivo de organizar e definir as atividades, os papéis e responsabilidades no projeto de teste.
    O Projeto de Teste de Software é a especificação da abordagem dos testes que serão aplicados ao software, assim como a definição dos casos de teste associados.
    O Plano de Teste de Software é o documento que apresenta o planejamento da execução dos testes do software, incluindo a definição da abrangência, dos recursos utilizados, das abordagens escolhidas e o cronograma de atividades.
<p><font color="red">Nota 0,5</font></p>
   2. (**0,5 ponto**) Descreva o relacionamento existente entre estes conceitos.
   O Projeto de Teste assim como o Plano de Teste de Software são artefatos resultantes de atividades definidas dentro das fases do Processo de Teste de Software. Pode-se dizer que tanto o Projeto de Teste como o Plano de Teste de Software estão contidos no Processo de Teste de Software.
<p><font color="red">Nota 0,0</font></p>

2. (**1,0 pontos**) Descreva as vantagens para a equipe de desenvolvimento ao se adotar um processo de teste ágil.
Um processo de teste ágil atua durante todo o ciclo de desenvolvimento do software, desde o planejamento, desenvolvimento e até a entrega das funcionalidades. Com uma visão sistêmica, os testadores buscam verificar se o que foi entregue foi o melhor possível para o usuário, e não apenas encontrar bugs. A qualidade do software é resultado dos testes com foco no usuário e gerenciamento de prioridade, características dos testes ágeis.
<p><font color="red">Nota 0,5</font></p>
3. (**1,0 ponto**) Cite pelo menos três características do Teste Exploratório.
Os Testes Exploratórios não seguem padrão ou roteiro de teste documentado. Precisam usar da criatividade para reagir e alterar o curso diante dos dados obtidos. Os casos de teste, a documentação dos teste e seus resultados são obtidos enquanto os testes são realizados.
<p><font color="red">Nota 1,0</font></p>
4. Considere os arquivos .java (Banco.java, Agencia.java, Conta.java e BankValidator.java). Nos próprios arquivos .java estão definidas as regras para cadastramento de cada um deles (Banco, Agencia e Conta). Desta forma, pede-se:
   1. (2.0 Pontos) Definir os cenários de teste suficientes para testar o cadastro e movimentações financeiras envolvendo bancos, agências e contas, conforme especificado. Para cada cenário definir os critérios de teste adequados à definição dos seus casos de teste.

        Agencia

        Número
        Critério - Número com 3 <= digitos <= 5, somente números

        C1 | Número com 1 digito | Erro
        C2 | Número com 2 digitos | Erro
        C3 | Número com 3 digitos | Acerto
        C4 | Número com 4 digitos | Acerto
        C5 | Número com 5 digitos | Acerto
        C6 | Número com 6 digitos | Erro
        C7 | Número com letra | Erro

        Nome
        Critério - Nome com 5 <= tamanho <= 100, somente letras

        C1 | Nome com 2 letras | Erro
        C2 | Nome com 5 letras | Acerto
        C4 | Nome com 101 letras | Erro
        C5 | Nome com caractere especial | Erro
        C6 | Nome com numero | Erro

        Cidade
        Critério - Cidade com 5 <= tamanho <= 100, somente letras

        C1 | Cidade com 2 letras | Erro
        C2 | Cidade com 5 letras | Acerto
        C4 | Cidade com 101 letras | Erro
        C5 | Cidade com caractere especial | Erro
        C6 | Cidade com numero | Erro

        Banco

        Número
        Critério - Número com 3 digitos, somente números

        C1 | Número com 1 digito | Erro
        C2 | Número com 2 digitos | Erro
        C3 | Número com 3 digitos | Acerto
        C4 | Número com 4 digitos | Erro
        C5 | Número com letra | Erro

        Nome
        Critério - Nome com 5 <= tamanho <= 100, somente letras

        C1 | Nome com 2 letras | Erro
        C2 | Nome com 5 letras | Acerto
        C4 | Nome com 101 letras | Erro
        C5 | Nome com caractere especial | Erro
        C6 | Nome com numero | Erro

        Conta

        Número
        Critério - Número com 6 digitos, somente números

        C1 | Número com 1 digito | Erro
        C2 | Número com 2 digitos | Erro
        C3 | Número com 3 digitos | Erro
        C4 | Número com 4 digitos | Erro
        C5 | Número com 5 digitos | Erro
        C6 | Número com 6 digitos | Acerto
        C7 | Número com 7 digitos | Erro
        C8 | Número com letra | Erro

<p><font color="red">Nota 1,0</font></p>

   2. (2.0) Definir os casos de teste suficientes para a cobertura do teste de cada um dos cenários definidos. Documentar os casos de teste no seguinte padrão:
   |CT|Valores de Entrada|Resultado esperado|

      Agencia

        Número

        CT1 | 0 | Erro
        CT2 | 11 | Erro
        CT3 | 123 | Acerto
        CT4 | 1234 | Acerto
        CT5 | 12345 | Acerto
        CT6 | 333444 | Erro
        CT7 | 1A23 | Erro

        Nome

        CT1 | Ag | Erro
        CT2 | Agencia | Acerto
        CT3 | Agência Itau Rua Juliana de Oliveira, Qdr. 195 - Lote 17 - St. Morada do Sol, Goiânia - GO, 74475-115 | Erro
        CT4 | Agencia - Itau | Erro
        CT5 | Agencia 01 | Erro

        Cidade

        CT1 | Ci | Erro
        CT2 | Goiás | Acerto
        CT3 | Agência Itau Rua Juliana de Oliveira, Qdr. 195 - Lote 17 - St. Morada do Sol, Goiânia - GO, 74475-115 | Erro | Erro
        CT4 | Goiás-Velho | Erro
        CT6 | Goiás1 | Erro

        Banco

        Número

        CT1 | 1 | Erro
        CT2 |12 | Erro
        CT3 | 123 | Acerto
        CT4 | 1234 | Erro
        CT5 | 12A | Erro

        Nome

        CT1 | Ba | Erro
        CT2 | Banco | Acerto
        CT3 | Agência Itau Rua Juliana de Oliveira, Qdr. 195 - Lote 17 - St. Morada do Sol, Goiânia - GO, 74475-115 | Erro
        CT4 | Banco! | Erro
        CT5 | Banco11 | Erro

        Conta

        Número

        CT1 | 0 | Erro
        CT2 | 00 | Erro
        CT3 | 000 | Erro
        CT4 | 0001 | Erro
        CT5 | 00001 | Erro
        CT6 | 000111 | Acerto
        CT7 | 0000001 | Erro
        CT8 | 00000A | Erro
<p><font color="red">Nota 0,5</font></p>

   3. (3.0 Pontos) Implementar (na linguagem de programação java) as classes para o teste da criação dos objetos e das movimentações financeiras envolvendo bancos e agências e contas.
<p><font color="red">Nota 0,0, os arquivos enviados são os mesmos compartilhados pelo professor. Não foram enviadas classes de teste.</font></p>

INSTRUÇÕES:
1. Tipo: Prova individual;
2. Local de Entrega: Plataforma Turing.
3. Forma de Entrega: arquivo compactado contendo:
   1. Este arquivo md, respondido.
   2. Classes de teste para (BancoTest, AgenciaTest e ContaTest);
   3. O arquivo compactado deverá ter o seguinte nome prova_p2<mat>.zip, onde mat é o número da matrícula do aluno(a).
5. Data da Entrega: 12/04/2022, as 22hs.
6. Critério de Aceitação: arquivo entregue, conforme solicitado.
7. Obs: segue no mesmo pacote o arquivo "org.apache.commons.lang.StringUtils", que é uma dependência do projeto. É deve ser inserida no _classpath_ do projeto de implementação da questão 4, caso não esteja utilizando o _maven_.

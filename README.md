# Praticando-JS_9
Media de Notas

Dentro do código está descrito como anotação, o exercicio que foi pedido. Logo em baixo,
os códigos que usei para resolve-lo!
Fique a vontade para entrar em contato comigo para dar sugestões e dicas!
Este e todos os outros exercícios foram tirados do curso
"Web Moderno Completo com JavaScript 2022 + Projetos" na Udemy.


Nesse código, temos algumas variáveis e uma função que realiza a classificação de notas de acordo com uma política específica. Vou explicar o código passo a passo:

1. São declaradas algumas variáveis:
   - `notaMedia`: Representa a média necessária para um aluno ser aprovado. Neste caso, o valor é 40.
   - `notaMinimaSemArredontamento`: Representa a nota mínima necessária para um aluno ser aprovado sem arredondamento. Neste caso, o valor é 38.
   - `aluno1`, `aluno2`, `aluno3`, `aluno4`, `aluno5`: Representam as notas dos alunos. Esses valores podem ser ajustados para diferentes alunos.

2. Em seguida, temos a função chamada `classificacao`, que recebe uma nota como parâmetro e retorna a classificação correspondente com base nas regras definidas.

3. Dentro da função `classificacao`, são calculadas duas variáveis:
   - `proximoMultiplo`: É calculado como o próximo múltiplo de 5 maior ou igual à nota fornecida pelo aluno. Isso é feito dividindo a nota por 5 e arredondando o resultado para cima utilizando `Math.ceil()`.
   - `diferenca`: É calculada como a diferença entre o próximo múltiplo de 5 e a nota do aluno.

4. Em seguida, são aplicadas as seguintes condições:
   - Se a nota do aluno for menor que a média (`notaMedia`), a função retorna a string "Reprovado".
   - Caso contrário, se a diferença entre o próximo múltiplo de 5 e a nota for menor que 3, a função retorna o próximo múltiplo de 5.
   - Caso contrário, se a nota do aluno for maior que a diferença, a função retorna a string "Aprovado".

5. Por fim, o código chama a função `classificacao` para cada aluno (`aluno1`, `aluno2`, etc.) e imprime o resultado no console usando `console.log`.

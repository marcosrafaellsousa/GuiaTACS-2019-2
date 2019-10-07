# Código-Fonte
Este é um guia do desenvolvedor escrito para disciplina Técnicas avançadas de Construção de Software, disponibilizada no segundo semestre de 2019 para os alunos da UFG cursando Engenharia de Software. O propósito desse guia é concretizar os conhecimentos e lições aprendidos em sala e nos materiais de estudo. 
Inicialmente esse guia apontará boas práticas em relação a criação de código-fonte limpo.

# Criando nomes úteis

Desenvolvedores criam nome o tempo todo, nome de pacotes, arquivos, funções, variáveis, os nomes em um software possuem um grande peso na sua legibilidade um dos fatores que definem a manutenibilidade, mal é preciso dizer, manutenções são operações constantes que mantém um software vivo, na maioria dos casos a manutenção já é cara e a manutenibilidade do software só piora ao longo das manutenções, um processo natural porém que pode ser desacelerado e barateado.

## O que levar em consideração na hora de criar nomes

- Escolher nomes úteis que carregam significado (pra que existe, o que faz)
- Caso não seja possível criar um nome satisfatório crie um placeholder com o máximo de informação possível
- Mude os nomes quando achar melhores
- Pense no contexto. Quem vai tirar valor daquela informação?
> Esta pessoa já possui um certo nível de formação?
- Contexto da linguagem e das tecnologias.
> Por exemplo, se a linguagem for fortemente tipada, uma variável nomeString é redundante, pois o código já diz que a variável é do tipo string, parâmetros de funções também podem ser utilizados para o entendimento daquele método, se uma função tem o nome "converterParaDias" e recebe um parâmetro chamado "minutos" já é entendido que a função converte minutos para dias.
- Evitar palavras que já possuem um uso comum
> Palavras como "Tabela" já tem um significado muito forte dentro do desenvolvimento de software, se referindo a tabelas de banco de dados relacionais, o uso dessas palavras pode levar a informação mal orientada. "Lista" também é uma estrutura de dados bem comum e deve-se evitar o uso dela se a estrutura não for uma lista.
- Evitar abreviações e criar nomes que podem ser pronunciados.
- É preferível mudar o nome da implementação ao invés da interface
> Por exemplo uma interface "CarrinhoDeCompras" é comumente chamada de "ICarrinhoDeCompras", porém uma opção melhor é de chamá-la de "CarrinhoDeCompras" e sua implementação de "CarrinhoDeComprasImp".
- Classes devem ter nomes de substantivos
- Funções devem ter nome de verbos
- Evitar nomes diferentes para o mesmo conceito
> "numero" e "decimal" podem se referir a mesma coisa, porém deve-se escolher um dos métodos para seguir em todas os nomes para evitar interpretações equivocadas
- Evite ambiguidade
> Uma palavra deve servir apenas a uma finalidade, por exemplo, se existem vários métodos "add" em classes diferentes, que adicionam um objeto a uma lista, e você faz um novo método que soma dois valores, "add" não é o mais adequado, pois cria ambiguidade sobre o que "add" faz, ao invés disso use um nome novo que não está sendo utilizado ainda "sum" por exemplo.
- Use um padrão de nomeclatura
> Geralmente cada linguagem tem uma padrão de nomenclatura para métodos, variáveis, classes, constantes, conheça o padrão mais utilizado por sua linguagem.

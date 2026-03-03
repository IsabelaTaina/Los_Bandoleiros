Primeiro grupo - Variáveis (declarativas, inferências)

Quando declarar uma  variável sem um valor definido é recomendado usar a declarativa em vez de var.
No geral sempre definir 
Object objeto = null; Pode?

Segundo grupo - Dynamic

Dynamic - nao verifica o tipo da variavel, o Dart ignora e dessa forma não dá erro.
Não garante previsibilidade;
Adequado somente em casos específicos.
Não consegue validar, se colocar uma função inexistente não mostra o erro de compilação.

- final: normalmente usa em objetos de classes que não sei os atributos
- Nesses casos de listas e classes ele não torna o conteúdo imutável, mas torna a referência para o endereço.

- const: o valor é fixo e deve ser definido antes da compilação.

Grupo 3 - Paramêtros Posicionais

- Posicionais: A função segue a ordem dos paramêtros definidos.
- Opcionais: Torna um parâmetro opcional, determinado por "[]", se nenhum valor for passado ele gera um valor padrão (null).
Caso nenhum valor seja passado, ele vai imprimir apenas o paramêtro definido.
Pode ser passado um valor diretamente dentro do paramêtro opcional.
-Nomeados: 



#atividade REGEX - 06/05

 Foi implementado um formulário de cadastro em HTML com algumas validação de campos. A explicação de como funciona cada uma delas esta logo abaixo!

Expressão para validação do Nome:
regex
Copy code
/^[^\d]{1,100}$/
^: Indica o início da string.
[^\d]: Representa qualquer caractere que não seja um dígito (0-9).
{1,100}: Limita o comprimento do nome entre 1 e 100 caracteres.
$: Indica o fim da string.
Essa expressão garante que o campo do nome não contenha números e tenha no máximo 100 caracteres.

Expressão para fazer a validação do Email:
regex
Copy code
/^[^\s@]+@[^\s@]+\.[^\s@]+$/
^: Indica o início da string.
[^\s@]+: Representa um ou mais caracteres que não sejam espaços em branco (\s) ou o símbolo "@".
@: Indica a presença do símbolo "@".
[^\s@]+: Representa um ou mais caracteres que não sejam espaços em branco (\s) ou o símbolo "@".
\.: Indica a presença de um ponto (".") para separar o nome de domínio.
[^\s@]+: Representa um ou mais caracteres que não sejam espaços em branco (\s) ou o símbolo "@".
$: Indica o fim da string.
Essa expressão valida se o email inserido possui um formato válido.

Expressão para Validar o Número de Telefone:
regex
Copy code
/^\d{2}\d{4,5}\d{4}$/
^: Indica o início da string.
\d{2}: Representa dois dígitos, correspondentes ao DDD do telefone.
\d{4,5}: Representa 4 ou 5 dígitos, que podem ser o número do telefone (caso de 8 ou 9 dígitos no total).
\d{4}: Representa quatro dígitos, correspondentes ao número do telefone.
$: Indica o fim da string.
Essa expressão verifica se o número de telefone inserido está com o DDD seguido do número.

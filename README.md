# Como utilizar

No diretório imediatamente acima do seu módulo, execute:

`git clone https://github.com/Danielbano1/curso`

Depois você pode utilizar as funções de curso com o import:

```Python
from .. import curso

curso.get_curso(25)
```

**OBS:** Para utilizar imports relativos, seu módulo também precisa fazer parte de um package, ou seja, o diretório do módulo deve possuir um arquivo `__init__.py` assim como o nosso.

Alternativamente, se o diretório acima do seu módulo também for um repositório, como o principal, você pode adicionar curso como submódulo:

`git submodule add https://github.com/Danielbano1/curso`

## Dependências

Python 3.9+

# Documentação adicional

O módulo possui um endereço de um arquivo fixo para registro da base de dados em memória persistente, inacessivel ao cliente.
O módulo usa um espaço em memória de acesso rápido para guardar o banco de dados para o uso das funcionalidades do módulo. Esta posição de memória também é inacessível ao cliente.

## inicializar

Esta função realiza a leitura da base de dados na memória persistente para um espaço de acesso rápido a ser usado pelas outras funções. A memória de acesso rápido acessada é fixa e qualquer informação previamente armazenada será perdida.

### Requisitos

- Retorna ARQUIVO_NAO_ENCONTRADO caso não encontre o arquivo de leitura
- Retorna ARQUIVO_EM_FORMATO_INVALIDO caso encontre o arquivo de leitura, mas não seja capaz de fazer a leitura
- Retorna OPERACAO_REALIZADA_COM_SUCESSO caso faça a leitura com sucesso
- Não avalia a integridade do conteudo lido e sua compatibilidade com as aplicações que o usarão

## finalizar

Esta função realiza o registro da base de dados em memória de acesso rápido sendo usada pelo módulo no arquivo resignado pelo módulo. Qualquer conteudo prévio no arquivo será sobrescrito.

### Requisitos

- Retorna

## get_curso

## get_cursos

## add_curso

## del_curso









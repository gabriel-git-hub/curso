# Como utilizar

No diretório imediatamente acima do seu módulo, execute:

`https://github.com/Danielbano1/curso`

Depois você pode utilizar as funções de curso com o import:

```Python
from .. import curso

curso.get_curso(25)
```

**OBS:** Para utilizar imports relativos, seu módulo também precisa fazer parte de um package, ou seja, o diretório do módulo deve possuir um arquivo `__init__.py` assim como o nosso.

Alternativamente, se o diretório acima do seu módulo também for um repositório, como o principal, você pode adicionar turma como submódulo:

`git submodule add https://github.com/Danielbano1/curso`

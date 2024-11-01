# playwright-python

## Install the Pytest plugin:

```bash
pip install pytest-playwright
```

## Install the required browsers:

```bash
playwright install
```

## Running the Example Test

By default tests will be run on chromium. This can be configured via the CLI options. Tests are run in headless mode meaning no browser UI will open up when running the tests. Results of the tests and test logs will be shown in the terminal.

```bash
pytest
```

Executar testes no headfull

Para executar seus testes no modo head, use o --headed flag. Isso abrirá uma janela do navegador enquanto executa seus testes e, uma vez finalizada, a janela do navegador será fechada.

```bash
pytest --headed
```

Execute testes em diferentes Navegadores

Para especificar em qual navegador você deseja executar seus testes, use o --browsersinalizador seguido do nome do navegador.

```bash
pytest --browser webkit
```

Para especificar vários navegadores para executar seus testes, use o --browser sinalizador várias vezes seguido pelo nome de cada navegador.

```bash
pytest --browser webkit --browser firefox
```

Execute 
Para executar um único arquivo de teste, passe o nome do arquivo de teste que você deseja executar.

```bash
pytest test_login.py
```

Para executar um teste específico, passe o nome da função do teste que você deseja executar.

```bash
pytest -k test_add_a_todo_item
```

Executar testes em Paralelo

Para executar seus testes em paralelo, use o --numprocesses flag seguido pelo número de processos nos quais você gostaria de executar seus testes. Recomendamos metade dos núcleos lógicos da CPU.

```bash
pytest --numprocesses 2
```

Gravando um trace

Os rastros podem ser registrados executando seus testes com o --tracingsinalizador.

```bash
pytest --tracing on
```

Abrindo o trace

```bash
playwright show-trace trace.zip
```

## Updating Playwright

To update Playwright to the latest version run the following command:

```bash
pip install pytest-playwright playwright -U
```

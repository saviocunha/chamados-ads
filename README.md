# Chamados ADS


## Objetivo 
Criar a estrutura inicial de uma API de chamados de suporte com Flask. Atividade desenvolvida na disciplina de **Programação para a Web** (curso de Análise e Desenvolvimento de Sistemas — UFCA), sob orientação do Prof. Dr. Jayr Alencar Pereira.

## Aluno

- **Nome:** Francisco Sávio Sousa da Cunha
- **E-mail:** savio.cunha@aluno.ufca.edu.br
- **Curso:** ADS - UFCA
- **Repositório:** https://github.com/saviocunha/chamados-ads

## Tecnologias

- Python 3.14
- Flask
- uv (para instalar as dependências e rodar o projeto)

## Como rodar

Primeiro clone o repositório e entre na pasta:

```bash
git clone https://github.com/saviocunha/chamados-ads.git
cd chamados-ads
```

É recomendado usar um ambiente virtual para não misturar as dependências do projeto
com as do sistema. 

```bash
python3 -m venv .venv
source .venv/bin/activate        # Linux/macOS
# .venv\Scripts\activate         # Windows
```

Instale o uv.

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Instale as dependências:

```bash
uv sync --lock
```

Rode o projeto:

```bash
uv run flask --app app run
```

Aí é só abrir **http://127.0.0.1:5000** no navegador.

Para encerrar a aplicação pressione CTRL + C.

Para sair do ambiente virtual depois, é só rodar `deactivate`.

## Rotas

Por enquanto só existe uma:

| Método | Rota | Retorno |
| --- | --- | --- |
| GET | `/` | `{"mensagem": "API em funcinamento"}` |


## Licença

MIT.

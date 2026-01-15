# 🐍 Python Project Cheatsheet (uv)

Cheatsheet rápido para criação, gerenciamento e execução de projetos Python usando **uv** — gerenciador moderno de dependências e ambientes virtuais.

---

## 📦 Download:
```bash
$ curl -Ls https://astral.sh/uv/install.sh | sh
```

Verificar instalação:
```
$ uv --version
```

---

## 🚀 Criando um novo projeto
```
$ uv init meu-projeto
```
Obs.: É possível iniciar o projeto sem um nome também, ex: 
```
$ uv init
```

## Estrutura padrão do projeto:
```
meu-projeto/
├── pyproject.toml
├── .python-version
├── README.md
└── src/
    └── meu_projeto/
        └── __init__.py
```
---

## Para adicionar lib no projeto:
```
$ uv add fastapi
```
## Adicionando em um ambiente específico:
```
$ uv add --dev fastapi
```

## Para remover uma lib:
```
$ uv remove fastapi
```

As dependências serão adicionadas ou removidas do pyproject.toml;

---

## Para rodar arquivos python direto:
```
$ uv run main.py
```
### Listagem de versões do python no sistema:
```
$ uv python list
```
### Instalar versão específica do python:
```
$ uv python install 3.12
```
### Definir versão específica no projeto:
```
$ uv python pin 3.12
```
### Sincronizar todas as libs que estão no pyproject.toml:
```
$ uv sync 
```
### Para instalar dependências do pip(requirements.txt) via uv:
```
$ uv install -r requirements.txt
```


---
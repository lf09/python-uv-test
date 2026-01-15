# 🐍 Python Project Cheatsheet (uv)

Cheatsheet rápido para criação, gerenciamento e execução de projetos Python usando **uv** — gerenciador moderno de dependências e ambientes virtuais.

---

## 📦 Download:
```bash
$ curl -Ls https://astral.sh/uv/install.sh | sh

Verificar instalação:
$ uv --version

## 🚀 Criando um novo projeto
$ uv init meu-projeto
Obs.: É possível iniciar o projeto sem um nome também, ex: 
$ uv init

## Estrutura padrão do projeto:
meu-projeto/
├── pyproject.toml
├── .python-version
├── README.md
└── src/
    └── meu_projeto/
        └── __init__.py

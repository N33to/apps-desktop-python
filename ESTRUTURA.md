# Estrutura do projeto

Mapa das pastas e arquivos de código. O código-fonte não é publicado neste repositório
(é software de uso interno de uma empresa real); aqui fica a arquitetura.

```text
├── financeiro/   # controle financeiro local (SQLite)
│   ├── app/
│   │   ├── web/
│   │   │   ├── app.css
│   │   │   ├── app.js
│   │   │   └── index.html
│   │   ├── banco.py
│   │   ├── catalogo.py
│   │   ├── config.py
│   │   ├── formatos.py
│   │   ├── gui.py
│   │   ├── importacao.py
│   │   ├── lancamentos.py
│   │   ├── lista_simples.py
│   │   ├── listas.py
│   │   ├── main.py
│   │   ├── planilha_antiga.py
│   │   ├── relatorios.py
│   │   ├── tema.py
│   │   ├── web_api.py
│   │   └── web_janela.py
│   ├── scripts/
│   │   ├── conferir_web.py
│   │   ├── dados_de_exemplo.py
│   │   ├── gerar_planilha.py
│   │   └── rebuild.py
│   └── tests/
│       ├── comum.py
│       ├── test_banco_e_listas.py
│       ├── test_formatos.py
│       ├── test_gui.py
│       ├── test_lancamentos.py
│       ├── test_lista_simples.py
│       ├── test_planilha_antiga.py
│       ├── test_relatorios_e_importacao.py
│       └── test_web_api.py
└── ponto-e-termos/   # ponto mensal, horas extras e termos em PDF
    ├── app/
    │   ├── web/
    │   │   ├── app.css
    │   │   ├── app.js
    │   │   └── index.html
    │   ├── banco.py
    │   ├── config.py
    │   ├── empresas.py
    │   ├── gui.py
    │   ├── main.py
    │   ├── office.py
    │   ├── ponto.py
    │   ├── ponto_dados.py
    │   ├── ponto_ficha.py
    │   ├── ponto_importar.py
    │   ├── ponto_relatorio.py
    │   ├── ponto_valores.py
    │   ├── scanner.py
    │   ├── tema.py
    │   ├── termos.py
    │   ├── web_api.py
    │   └── web_janela.py
    ├── scripts/
    │   ├── conferir_web.py
    │   └── rebuild.py
    └── tests/
        ├── test_banco.py
        ├── test_empresas.py
        ├── test_ponto.py
        ├── test_ponto_dados.py
        ├── test_ponto_ficha.py
        ├── test_ponto_importar.py
        ├── test_ponto_relatorio.py
        ├── test_ponto_valores.py
        ├── test_termos.py
        └── test_web_api.py
```

## Tamanho (linhas, sem bibliotecas de terceiros)

| Linguagem | Linhas |
|---|---:|
| Python | 22.987 |
| JavaScript | 1.800 |
| CSS | 578 |
| HTML | 358 |

_Arquivos: 63._

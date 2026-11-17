# Aplicativos de mesa em Python: financeiro e ponto

Dois programas Windows locais que automatizaram rotinas de uma empresa antes de existir o [ERP web](https://github.com/N33to/erp-gestao-empresarial), que depois absorveu as duas funções.

> **O código e os dados não são públicos** (são cadastros e contabilidade reais). Este repositório traz a arquitetura em [ESTRUTURA.md](ESTRUTURA.md).

## `financeiro/`: controle financeiro

Lançar pagamentos e recebimentos, acompanhar vencimentos e emitir relatórios de semana, mês e ano, com exportação para Excel.

- **Dinheiro em centavos inteiros** e datas ISO no banco (SQLite em modo WAL).
- **Três regimes de relatório** (caixa, competência e vencimento), com teste que trava a diferença entre eles.
- **Importação com reconhecimento automático de formato** (planilha antiga de controle, planilha de listas e listas simples), com **simulação antes de gravar** e **desfazer por lote**.
- **Parcelamento sem erro silencioso:** a soma das parcelas é sempre igual ao total, travado por teste.
- **193 testes automatizados.**

## `ponto-e-termos/`: ponto mensal e termos

Digitação do cartão de ponto, apuração de horas extras, valor em reais com DSR, ficha em PDF e geração em lote de termos mensais.

- **Regra de 65/75/100% transcrita das fórmulas da planilha original** e conferida dia a dia: dos 372 dias de um mês de referência, 362 bateram; as 10 diferenças eram células digitadas por cima da fórmula, e ficaram documentadas em testes.
- **Valores arredondados por faixa, em centavos**, para o total fechar na calculadora de quem confere.
- **Salário e divisor congelados por competência**, para que um reajuste novo não altere o fechamento de um mês antigo.
- **Ficha em PDF idêntica ao cartão** usado antes, com medidas lidas da planilha original.
- **354 testes automatizados.**

## Stack

Python 3.12 · SQLite · openpyxl · pywebview (WebView2) · HTML/CSS/JS · Word/Excel via COM · PyInstaller · Git

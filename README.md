# Agregador de Dados – Imposto de Renda (Excel)

Ferramenta desenvolvida em Excel para organizar e reunir as informações necessárias à declaração de Imposto de Renda Pessoa Física (IRPF), com navegação por menu, validação automática de dados e cálculo de totais.

## Objetivo

Centralizar em uma única planilha os dados que normalmente estão espalhados (recibos, informes de rendimento, comprovantes de despesas, bens etc.), reduzindo erros de digitação e facilitando a conferência antes do preenchimento do programa oficial da Receita Federal.

## Estrutura do arquivo

O arquivo é dividido em 7 abas:

| Aba | Conteúdo |
|---|---|
| **Início** | Menu de navegação com links diretos para cada aba e atalhos úteis (site da Receita Federal, consulta de restituição, perguntas frequentes) |
| **Dados_Pessoais** | Dados cadastrais do titular da declaração (nome, CPF, endereço, estado civil etc.) |
| **Dependentes** | Cadastro dos dependentes, com grau de parentesco e data de nascimento |
| **Rendimentos** | Rendimentos recebidos no ano, por fonte pagadora, tipo e imposto retido (IRRF) |
| **Despesas** | Despesas dedutíveis (saúde, educação, previdência, pensão alimentícia etc.) |
| **Bens_e_Direitos** | Bens e direitos declarados, com valor de 31/12 do ano anterior e do ano atual |
| **Resumo** | Totais consolidados, calculados automaticamente a partir das demais abas |

## Como usar

1. Abra o arquivo .
2. Comece pela aba **Início** e navegue pelos links até a seção desejada.
3. Preencha apenas as **células destacadas em amarelo** — são os campos de entrada de dados.
5. Os **totais são calculados automaticamente** por fórmula — não é necessário (e não é recomendado) editar as células de total.
6. Consulte a aba **Resumo** para visualizar todos os totais consolidados de uma vez.

## Funcionalidades

- **Menu de navegação**: links de hiperlink entre as abas, sem necessidade de rolar ou clicar nas guias.
- **Validação automática de dados**: uso de `Data Validation` do Excel para:
  - Restringir campos como UF, estado civil, tipo de rendimento e categoria de despesa a listas predefinidas;
  - Validar datas (ex.: data de nascimento).
- **Cálculo automático de totais**: uso de fórmulas nativas do Excel (`SUM`, `COUNTA`) para:
  - Somar rendimentos e imposto retido;
  - Somar despesas dedutíveis por categoria;
  - Contar o número de dependentes;
  - Calcular a variação patrimonial (bens do ano atual menos ano anterior);
  - Estimar a base de cálculo (rendimentos − deduções).
- **Links rápidos**: atalhos para páginas oficiais da Receita Federal na aba Início.
- **Formatação padronizada**: fontes, cores e bordas consistentes em todas as abas, com destaque visual para células de entrada (amarelo) e células de total (verde).

## Observações importantes

- Os valores apresentados na aba **Resumo** são **estimativas simplificadas** para fins de organização pessoal, **sem caráter oficial**.
- O cálculo definitivo do imposto devido deve ser feito exclusivamente no programa oficial da Receita Federal (IRPF).
- A planilha não substitui orientação de um contador ou profissional especializado.

## Tecnologia utilizada

- Microsoft Excel (formato `.xlsx`)
- Recursos nativos: fórmulas, validação de dados (`Data Validation`), hiperlinks internos, formatação condicional visual

## Autor

Desenvolvido como parte de um desafio prático de organização de dados em Excel por Jessica Aparecida Candido.

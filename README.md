[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-blue.svg)](https://creativecommons.org/licenses/by/4.0/)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)

# Sistema Adaptativo Baseado em Regras para o Ensino de Programação em Python

---

## Descrição Geral do Artigo

Este repositório apresenta os materiais, códigos e análises utilizados no estudo **“Sistema Adaptativo Baseado em Regras para o Ensino de Programação em Python: Um Estudo Experimental”**.

A proposta investiga a utilização de um sistema adaptativo simples, implementado com Google Forms e lógica baseada em regras, para personalizar o percurso de aprendizagem de estudantes da educação básica em um curso introdutório de programação em Python.

---

## Objetivo do Projeto

O objetivo do sistema é adaptar o percurso de aprendizagem dos estudantes com base em seu desempenho ao longo do curso, direcionando-os para:

* Progressão contínua;
* Atividades de reforço.

A proposta busca demonstrar que sistemas adaptativos simples e de baixo custo podem contribuir para:

* Personalização da aprendizagem;
* Apoio a estudantes com dificuldades;
* Redução de desigualdades educacionais;
* Melhoria da experiência do usuário.

---

## Estrutura do Curso

O curso foi organizado em oito tópicos sequenciais:

| Tópico | Conteúdo                                       |
| ------ | ---------------------------------------------- |
| T1     | Variáveis e Tipos de Dados                     |
| T2     | Operadores Aritméticos e Lógicos               |
| T3     | Estruturas Condicionais (`if`, `else`, `elif`) |
| T4     | Laços de Repetição (`for` e `while`)           |
| T5     | Funções em Python                              |
| T6     | Listas e Tuplas                                |
| T7     | Dicionários                                    |
| T8     | Entrada e Saída de Dados + Tratamento de Erros |


Ao final de cada tópico, o estudante respondia a uma questão avaliativa:

* Acerto → próximo tópico;
* Erro → conteúdo de reforço + nova atividade.

---

## Funcionamento do Sistema Adaptativo

O sistema foi implementado utilizando:

* Google Forms;
* Google Sheets;
* Lógica baseada em regras.

O modelo adaptativo funciona de forma simples:

1. O estudante realiza uma atividade;
2. O sistema verifica o desempenho;
3. Em caso de erro:
   - Apresenta feedback;
   - Libera conteúdo complementar;
   - Aplica nova questão.
4. Em caso de acerto:
   - Permite progressão no curso
---

## Estrutura do Repositório

```
├── LICENSE
│
├── README.md
│
├── curso_python_adaptativo.ipynb
│
└── python_adaptativo.xlsx
```

### Dataset

O conjunto de dados contém informações referentes ao desempenho dos participantes durante o curso.

Principais variáveis:

| Variável          | Descrição                        |
| ----------------- | -------------------------------- |
| `nota_pret`       | Nota do pré-teste                |
| `nota_post`       | Nota do pós-teste                |
| `ganho_bruto`     | Diferença entre pós e pré        |
| `ganho_hake`      | Ganho normalizado                |
| `qtd_reforcos`    | Quantidade de reforços acessados |
| `acertos_topicos` | Total de acertos                 |
| `ux_01` a `ux_05` | Itens da experiência do usuário  |
| `ux_media`        | Média geral de UX                |
---

### Análises Realizadas

O estudo inclui:

* Estatística descritiva;
* Testes de normalidade;
* Teste t de Student;
* Teste de Mann-Whitney;
* Correlação de Pearson e Spearman;
* Tamanho de efeito (Cohen’s d);
* Alfa de Cronbach;
* Análise de ganho normalizado de Hake
---

### Principais Resultados

Os resultados evidenciaram:

* Aumento significativo entre pré e pós-teste;
* Ganho médio relevante de aprendizagem;
* Elevada satisfação dos estudantes;
* Efeito de convergência entre grupos;
* Maior evolução relativa de estudantes com menor desempenho inicial.

Os achados sugerem que sistemas adaptativos baseados em regras podem atuar como mecanismo de suporte pedagógico e personalização da aprendizagem.

---

### Como Executar

1. Clone o repositório
```
git clone https://github.com/samteccmrj/pythonadaptativo.git
```

2. Instale as dependências
```
pip install pandas numpy scipy matplotlib openpyxl
```

3. Execute o script
```
python curso_python_adaptativo.ipynb
```
---

## Considerações Éticas

O estudo foi conduzido em conformidade com princípios éticos aplicáveis à pesquisa educacional envolvendo menores de idade.

Todos os participantes assinaram:

* TALE (Termo de Assentimento Livre e Esclarecido);
* TCLE assinado pelos responsáveis legais.

Os dados disponibilizados neste repositório encontram-se anonimizados.

---

## Ciência Aberta

Este repositório tem como objetivo promover:

* Transparência metodológica;
* Reprodutibilidade;
* Reutilização educacional;
* Replicação das análises.

Os materiais podem ser adaptados para diferentes contextos educacionais.

---

## Licença

Este projeto está disponibilizado sob a licença CC BY 4.0.

---

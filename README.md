# Projeto de Ciência de Dados e Inteligência Artificial: Análise de Crédito

Este projeto é sobre ciência de dados e Inteligência Artificial. Nele, desenvolvemos uma IA que realiza a análise de crédito automaticamente para os clientes listados na base de dados do banco. O objetivo é classificar os clientes em três categorias de score de crédito: **Ruim**, **Ok** e **Bom**.

## Objetivo
Criar um modelo de Inteligência Artificial que consiga analisar os dados de clientes de um banco e prever automaticamente o score de crédito com base em características como profissão, mix de crédito e comportamento de pagamento.

## Tecnologias Utilizadas
- [Python 3](https://www.python.org/)
- [Pandas](https://pandas.pydata.org/): Manipulação e análise de dados.
- [Scikit-learn](https://scikit-learn.org/): Criação e treinamento de modelos de aprendizado de máquina.

## Pré-requisitos
Certifique-se de ter o Python e as dependências necessárias instaladas. Para instalar os pacotes exigidos, execute o comando abaixo:

```bash
pip install pandas scikit-learn
```

# Base de Dados

As bases de dados utilizadas neste projeto incluem:

- **clientes.csv**: Dados de clientes do banco para análise e treinamento do modelo.
- **novos_clientes.csv**: Dados de novos clientes para previsões.

### Exemplo de estrutura da base de dados `clientes.csv`:

| id_cliente | profissao   | mix_credito | comportamento_pagamento | score_credito |
|------------|-------------|-------------|--------------------------|---------------|
| 1          | Engenheiro  | Completo    | Pontual                  | Bom           |
| 2          | Professor   | Parcial     | Atrasado                 | Ruim          |

---

## Passo a Passo do Projeto

1. **Entendimento do Desafio**  
   Analisar os clientes e definir o score de crédito com base nos dados fornecidos.

2. **Importação da Base de Dados**  
   Utilizamos a biblioteca `pandas` para importar e visualizar os dados.

3. **Preparação dos Dados**  
   As colunas categóricas (texto) foram convertidas para valores numéricos utilizando `LabelEncoder` da biblioteca `scikit-learn`.

4. **Treinamento do Modelo**  
   Dividimos os dados em conjunto de treino e teste para avaliar a precisão dos modelos. Dois modelos foram utilizados:
   - `Random Forest Classifier` (Árvore de Decisão)
   - `K-Nearest Neighbors` (KNN)

5. **Avaliação dos Modelos**  
   Comparamos a acurácia dos dois modelos e escolhemos o mais preciso.

6. **Previsão para Novos Clientes**  
   Aplicamos o modelo selecionado para prever o score de crédito de novos clientes.

---

## Como Executar

1. Certifique-se de que os arquivos `clientes.csv` e `novos_clientes.csv` estão no mesmo diretório que o arquivo `codigo.ipynb`.
2. Abra o arquivo `codigo.ipynb` em um ambiente como **Jupyter Notebook** ou **Google Colab**.
3. Siga os passos descritos no notebook para rodar o código e gerar as previsões.

---

## Resultados

- O modelo `Random Forest Classifier` foi escolhido com base na maior acurácia (83%).
- Previsões para novos clientes foram geradas utilizando o modelo selecionado.

---

## Possíveis Melhorias

- Testar outros algoritmos de classificação, como **Gradient Boosting** ou **SVM**.
- Adicionar mais dados à base para aumentar a robustez do modelo.
- Implementar técnicas de pré-processamento avançadas, como **normalização** ou **balanceamento de classes**.

---

## Autor

Este projeto foi desenvolvido por **Caio Oliveira Monteiro** em 2025, baseado em aulas ministradas durante a **Jornada Python da Hashtag**.

---

## Agradecimentos

Agradecemos ao professor **João Paulo de Lira** e à equipe da **Jornada Python da Hashtag** por fornecerem o conteúdo base para este projeto.

---

## Licença

Este projeto está licenciado sob a licença **MIT**. Sinta-se à vontade para usá-lo e modificá-lo conforme necessário.

___

Divirta-se explorando o mundo da Inteligência Artificial! 🚀

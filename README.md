<h1>
    <span> Projeto: Classificação de Aprovações de Alunos com Regressão Logística</span>
</h1>

Este projeto implementa um modelo de __Regressão Logística__ para prever se um aluno será aprovado ou reprovado com base em suas notas em duas disciplinas. O código utiliza bibliotecas do __Python__ como `pandas`, `scikit-learn` e `numpy` para manipulação de dados e aprendizado de máquina.

## Objetivo
O objetivo principal deste projeto é aplicar um modelo de aprendizado supervisionado para classificação, utilizando a regressão logística. O modelo prevê a aprovação de um aluno (1 para aprovado e 0 para reprovado) a partir de suas notas em duas matérias.

## Linguagem de Programação

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

## Estrutura do Projeto
- Manipulação de Dados: O conjunto de dados contém as notas de alunos e um indicador binário de aprovação. A manipulação dos dados é feita com `pandas`.
- Treinamento do Modelo: Utilizamos a regressão logística para treinar o modelo de classificação, que prevê se um aluno será aprovado ou não.
- Divisão dos Dados: O conjunto de dados é dividido em dois subconjuntos: 80% para treino e 20% para teste.
- Avaliação do Modelo: A performance do modelo é avaliada utilizando a métrica de __acurácia__.

## Dados
O conjunto de dados utilizado no projeto contém as seguintes colunas:

- Nota1: Nota do aluno na primeira disciplina.
- Nota2: Nota do aluno na segunda disciplina.
- Aprovado: Indica se o aluno foi aprovado (`1`) ou reprovado (`0`).
### Exemplo dos Dados:
```python
data = {
    'Nota1': [85, 62, 78, 95, 55, 40, 60, 90],
    'Nota2': [88, 65, 74, 90, 60, 42, 70, 85],
    'Aprovado': [1, 0, 1, 1, 0, 0, 0, 1]
}
````
## Instalação
Clone o repositório:
```python
git clone https://github.com/seu-usuario/seu-repositorio.git
```
## Instale as dependências:
```python
pip install -r requirements.txt
```
As principais bibliotecas utilizadas no projeto são:
- pandas
- scikit-learn
- numpy

## Como Executar
1. Certifique-se de que você está no diretório do projeto.
2. Execute o código do projeto:
```python
python main.py
```
O script __main.py__ carregará os dados, dividirá o conjunto de dados em treino e teste, treinará o modelo de Regressão Logística e exibirá a acurácia final do modelo.

## Acurácia do Modelo
Com os dados atuais, o modelo tem uma acurácia de __1.0__ (`100%`) no conjunto de teste, indicando que ele fez todas as previsões corretamente. No entanto, isso pode variar com diferentes divisões de dados.

## Questões Analisadas
- __Acurácia do Modelo:__ O modelo prevê corretamente as reprovações e aprovações dos alunos com base nas notas.
- __Superestimação/Subestimação:__ O modelo subestima as aprovações, pois não fez previsões de aprovação (classe 1) no conjunto de teste, mesmo que ele tenha acertado todas as reprovações.

## Melhorias Futuras
- __Balanceamento de Dados:__ Implementar técnicas de __subamostragem__ (`undersampling`) e __superamostragem__ (`oversampling`) para equilibrar o número de exemplos das classes `Aprovado` e `Reprovado`.
- __Validação Cruzada:__ Utilizar validação cruzada para avaliar a robustez do modelo em diferentes subconjuntos de dados.
- __Aumento de Dados:__ Incluir mais exemplos no dataset para melhorar a capacidade de generalização do modelo.

## Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request para melhorar o projeto.

## Licença
Este projeto está licenciado sob os termos da GNU General Public License v3.0. Consulte o arquivo LICENSE para mais detalhes.


## Observações:
- Substitua os links e nomes de usuário pelo seu próprio.
- Crie um arquivo `requirements.txt` com as dependências do projeto (`pandas`, `scikit-learn`, etc.). Você pode gerá-lo com o comando:
```python
pip freeze > requirements.txt
```





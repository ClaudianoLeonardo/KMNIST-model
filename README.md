
# Modelo de Classificação CNN para o Conjunto de Dados KMNIST

Este repositório contém um modelo de classificação de caracteres japoneses utilizando Redes Neurais Convolucionais (CNN) implementado em Python com o uso da biblioteca TensorFlow. O modelo é treinado e testado no conjunto de dados KMNIST, que é um conjunto de caracteres manuscritos do alfabeto Kuzushiji.

## Conjunto de Dados

Os dados para este projeto são baixados diretamente dos links fornecidos no código. Aqui está o script utilizado para baixar os dados:

```bash
# Baixando a base de dados
!wget http://codh.rois.ac.jp/kmnist/dataset/kmnist/kmnist-train-imgs.npz
!wget http://codh.rois.ac.jp/kmnist/dataset/kmnist/kmnist-train-labels.npz
!wget http://codh.rois.ac.jp/kmnist/dataset/kmnist/kmnist-test-imgs.npz
!wget http://codh.rois.ac.jp/kmnist/dataset/kmnist/kmnist-test-labels.npz
```

Os arquivos de treinamento e teste são baixados em formato `.npz` e contêm as imagens e rótulos correspondentes.

## Pré-requisitos

Para executar este projeto, você precisa ter o Python 3.x instalado, bem como as bibliotecas listadas no arquivo `requirements.txt`. Você pode instalá-las com o seguinte comando:

```bash
pip install -r requirements.txt
```

## Uso

O processo de treinamento e avaliação do modelo é dividido em várias etapas:

1. **Baixando a base de dados**: Os dados são baixados diretamente dos links fornecidos.
2. **Pré-processamento dos dados**: Os dados são normalizados e pré-processados para serem compatíveis com o modelo.
3. **Construindo o modelo**: Um modelo de CNN é criado usando a biblioteca TensorFlow.
4. **Treinamento do modelo**: O modelo é treinado com os dados de treinamento.
5. **Avaliação do modelo**: O desempenho do modelo é avaliado com os dados de teste.
6. **Exibição de resultados**: Os resultados do treinamento e a matriz de confusão são exibidos.

Você pode executar cada etapa seguindo o código fornecido no projeto.

## Estrutura do Repositório

- `data/`: Contém os dados brutos baixados do KMNIST.
- `src/`: Contém o código-fonte Python utilizado para baixar, pré-processar, treinar e avaliar o modelo.
- `requirements.txt`: Lista de dependências necessárias.
- `README.md`: Este arquivo.

## Resultados

Os resultados do modelo treinado são exibidos na seção "Avaliando performance do treinamento" do código, incluindo a precisão, matriz de confusão e o relatório de classificação.


## Licença

Este projeto é licenciado sob a Licença MIT. Consulte o arquivo [LICENSE.md](LICENSE.md) para obter mais informações.

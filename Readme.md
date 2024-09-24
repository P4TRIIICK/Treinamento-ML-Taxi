# Projeto de Aprendizado por Reforço - Taxi-v3

Este projeto implementa um agente de aprendizado por reforço que aprende a resolver o ambiente `Taxi-v3` do OpenAI Gym usando a técnica de **Q-learning**. O agente aprende a navegar pelo ambiente, pegando passageiros e deixando-os nos destinos corretos com o menor número de penalidades possível.

## Requisitos

- Python 3.x
- OpenAI Gym (versão 0.17.3)
- NumPy

## Instalação

1. Clone o repositório ou baixe o código.
2. Certifique-se de ter o Python 3.x instalado no sistema.
3. Instale as dependências do projeto com o seguinte comando:

    ```bash
    pip install -r requirements.txt
    ```

4. Para executar o projeto, utilize um ambiente Jupyter Notebook e rode o código por partes, pois o treinamento do agente envolve loops longos.

## Estrutura do Projeto

- **Treinamento Q-Learning**: O agente é treinado em 100.000 episódios para aprender as melhores ações para cada estado.
- **Avaliação**: Após o treinamento, o agente é testado em 50 episódios para medir o desempenho em termos de penalidades.

## Uso

- O código está otimizado para ser executado em um Jupyter Notebook.
- O treinamento leva algum tempo e você pode acompanhar o progresso pelo número de episódios treinados.
- Para interromper a exibição visual do ambiente ou finalizar o processo, pressione **Ctrl + C** ou interrompa manualmente no Jupyter.

## Tecnologias Utilizadas

- **Gym**: Para criar e gerenciar o ambiente de simulação do Taxi-v3.
- **NumPy**: Para a manipulação das tabelas Q usadas no algoritmo de Q-learning.

## Notas

- O ambiente de simulação do Taxi-v3 usa uma visualização em terminal simples. Para suprimir a interface gráfica, foi utilizado `os.environ["SDL_VIDEODRIVER"] = "dummy"`.
- O treinamento pode ser interrompido a qualquer momento, e a tabela Q resultante será usada para a avaliação do agente.

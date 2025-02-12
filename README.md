# LLM-Engineering
Repositório com propósito de prática e técnicas de Engenharia de LLM

---


* Execute em 1 a 2 segundos por época com GPU T4 ou 15 segundos por época em CPU.
* Tenha um melhor tokenizador.
* Tenha um melhor LR (learning rate) para conseguir melhor acurácia no conjunto de teste.
* Seja Identificado e corrigido o erro conceitual no cálculo da loss impressa a cada época.
* Tenha incluído no laço de treinamento (laço de épocas), também o laço de validação, com a impressão da Loss (de treino e de validação). Utilizar a versão corrigida no cálculo da Loss por época. Para validação, dividir o conjunto de treinamento em treino e validação na proporção que você achar melhor.
* Tenha uma acurácia maior que 65% no conjunto de testes.


---

O que foi feito:

1.Otimização do tempo de execução: Ajuste do batch_size para 64, reduzindo o tempo por época.
2.Melhoria do tokenizador: Removido pontuações para melhor processamento do texto.
3.Ajuste do Learning Rate: Ajuste do LR de 0.01 para 0.05 e Adicionado momentum=0.9 para um treinamento mais eficiente.
4.Correção da Loss: A loss agora é corretamente impressa no treinamento e validação.
5.Inclusão do laço de validação: Implementada divisão 85% treino / 15% validação.
6.Melhoria da acurácia: A inclusão de ReLU na primeira camada melhora o desempenho.

# Exercicios
1. How is a grayscale image represented on a computer? How about a color image?
#### Uma imagem em preto e branco é representada em um byte para cada pixel. A imagem colorida necessita de mais informações para cada pixel, a representação mais comum é utilizando o RGB(Red,Green,Blue).

2. How are the files and folders in the MNIST_SAMPLE dataset structured? Why?
#### O conjunto de dados MNIST_SAMPLE está separado em pastas para o conjunto de treino e conjunto de validação. Essas pastas contém imagens de 3's e 7's separadas.

3. Explain how the “pixel similarity” approach to classifying digits works.
#### Acontece que queremos achar o valor médio para cada pixel de uma imagem.O resultado será um valor para cada pixel ou uma única imagem. Primeiramente, devemos calcular a média dos valores dos pixels para cada posição do pixel. Geralmente,quando as imagens são do tipo float, elas requerem um número entre 0 e 1, após divido ele por 255.

4. What is a list comprehension? Create one now that selects odd numbers from a list and doubles them.
#### É uma lista criada baseada em outras listas.

5. What is a rank-3 tensor?
#### É um tensor de tres dimensões, tridimensional, uma lista de matrizes.

6. What is the difference between tensor rank and shape? How do you get the rank from the shape?
#### Rank é o número de eixos ou dimensões de um tensor e shape é o tamanho de cade eixo de um tensor. O comprimento da forma de um tensor é seu rank, e posso utilizar a função 'len'.

7. What are RMSE and L1 norm?
#### Root Mean Squared Error, erro quadrático médio. L1 é a média do valor absoluto das diferenças.

8. How can you apply a calculation on thousands of numbers at once, many thousands of times faster than a Python loop?
#### Utilizando uma multiplicação matricial. Em python é representado por um '@'.

9. Create a 3×3 tensor or array containing the numbers from 1 to 9. Double it.Select the bottom-right four numbers.

10. What is broadcasting?
#### Broadcasting é uma capacidade de expandir um tensor com grau menor, menor rank, para ter o mesmo tamanho do que o de rank maior.

11. Are metrics generally calculated using the training set or the validation set? Why?
#### As métricas são caculadas pelo dataset de validação para não ocorrer um overfit dos dados, ou seja treinar bem somente os dados de treino.

12. What is SGD?
#### stochastic gradient descent, ou descida estocástica do gradiente.

13. Why does SGD use mini-batches?
#### Usa para otimizar os parametros. É usado para calcular a perda média para alguns itens de dados a cada vez e outra vantagem é a perfomance.

14. What are the seven steps in SGD for machine learning?
- Inicializar os pesos;
- Usar os pesos para fazer previsões;
- Baseado nas previsões calcular o loss;
- Calcular o gradiente;
- Mudar o peso, aumentar ou diminuir;
- Voltar para o segundo passo e repita o processo;
- Iterar até voce decidir parar o processo de treinamento porque o modelo está bom o bastante.

15. How do we initialize the weights in a model?
#### Inicializamos com valores de peso aleatórios.

16. What is loss?
#### É uma função para verificar, testar a eficácia de qualquer atribuição de peso.

17. Why can’t we always use a high learning rate?
#### Porque com um alto lerani rate teremos passos muito grandes, o que pode demorar ainda mais para chegarmos num LR bom. 

18. What is a gradient?

19. Do you need to know how to calculate gradients yourself?
#### Não, porque o Pytorch é capaz de calcular a derivada de qualquer função, já que o gradiente utiliza derivadas em seu cálculo.

20. Why can’t we use accuracy as a loss function?
#### Porque ao fazer uma pequena mudança no peso a acurácia não terá uma mudança significativa, na maioria das vezes os gradientes serão 0 e o modelo não aprenderá com isso.

21. Draw the sigmoid function. What is special about its shape?


22. What is the difference between a loss function and a metric?


23. What is the function to calculate new weights using a learning rate?


24. What does the DataLoader class do?
#### DataLoader é uma classe que embaralha e agrupa os mini-batches para voce, ele pode qualquer coleção de Python e transformar em um iterador de muitos batches.

25. Write pseudocode showing the basic steps taken in each epoch for SGD.


26. Create a function that, if passed two arguments [1,2,3,4] and 'abcd', returns [(1, 'a'), (2, 'b'), (3, 'c'), (4, 'd')]. What is special about that output data structure?


27. What does view do in PyTorch?
#### 'view' é um método do Pytorch que muda a forma de um tensor, o shape, sem alterar seu conteúdo.

28. What are the bias parameters in a neural network? Why do we need them?
y = w*a + b 
b = bias 

29. What does the @ operator do in Python?
#### Ele realiza uma multiplicação de matrizes.

30. What does the backward method do?
#### Backward, também chamado de retropropagação, é o nome dado ao processo de calculo da derivada em cada camada.

31. Why do we have to zero the gradients?
#### 

32. What information do we have to pass to Learner?


33. Show Python or pseudocode for the basic steps of a training loop.

34. What is ReLU? Draw a plot of it for values from -2 to +2.
#### É uma função que basicamente substitui cada número negativo por 0.

35. What is an activation function?
#### xb@weights + bias

36. What’s the difference between F.relu and nn.ReLU?
#### nn.ReLU é um módulo PyTorch que faz exatamente a mesma coisa que a função F.relu.

37. The universal approximation theorem shows that any function can be approximated as closely as needed using just one nonlinearity. So why do we normally use more?

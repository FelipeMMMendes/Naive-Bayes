# Naive Bayes
Modelo Naive-Bayes para previsão de diabetes e previsão de categorias de produtos em e-commerce. 

### Sobre o Naive Bayes:

**Naive Bayes é um método probabilístico classificação para classificação**. Os métodos probabilísticos são técnicas matemáticas e estatísticas usadas para modelar, analisar e prever eventos que são incertos ou aleatórios. Ao contrário dos métodos determinísticos, que fornecem resultados exatos para um conjunto de entradas específico, os métodos probabilísticos lidam com a incerteza e fornecem uma gama de possívels resultados com diferentes probabilidades associadas.

Os métodos são aplicados em áreas tipo finanças, para prever o comportamento de preços de ações, ou na engenharia, nos projetos de sistemas que operam sob incertezas.

### Naive Bayes x Redes Neurais

![NaivexNN](https://i.imgur.com/IiC8IuG.png)

### Diferença entre métodos determinísticos e probabilísticos

**A principal diferença entre os métodos determinísticos e probabilísticos reside em como eles lidam com a incerteza.**

**Métodos Determinísticos**
- Produzem um único resultado ou solução para um conjunto específico de entradas.
- Baseiam-se na premissa de que o sistema ou problema é completamente conhecido e não há incerteza.

**Métodos Probabilísticos**:
- Fornecem uma gama de possíveis soluções ou resultados, cada um com uma probabilidade associada.
- São usados quando há incerteza no sistema ou problema, seja devido à falta de conhecimento, variação inerente ou ambos.

Os eventos e cenários do mundo real muitas vezes são incertos, então os métodos determinísticos podem levar a conclusões imprecisas, dessa forma, os métodos probabilísticos, ao reconhecerem e incorporarem essa incerteza, permitem uma modelagem e análise mais robusta.

A impportância dos métodos probabilísticos em cenários incertos inclui:

- **Tomada de Decisão Informada**: Esses métodos fornecem um leque de possíveis resultados com probabilidades associadas, as pessoas podem avaliar os riscos e benefícios de diferentes ações.

- **Robustez em Previsões**: Em vez de uma única previsão pontual, os métodos probabilísticos oferecem uma distribuição de possíveis resultados.

- **Otimização sob Incerteza**: Em problemas de otimização, os métodos probabilísticos podem ajudar a encontrar soluções que são robustas a variações ou incertezas no sistema.

### Como funciona o Naive Bayes?

Esse algoritmo é baseado no Teorema de Bayes, uma fórmula matemática que descreve como atualizar probabilidades com novas evidências. O algoritmo foi nomeado em homenagem ao reverendo Thomas Bayes, que forneceu a primeira fórmula para inferir a probabilidade de um evento A, dado o conhecimento prévio de eventos que podem estar relacionados a A.

A fórmula do Teorema de Bayes é:

O Teorema de Bayes descreve a probabilidade de um evento, baseado em conhecimento prévio de condições que possam estar relacionadas ao evento. A fórmula é:

\[ P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)} \]

onde:
- \( P(A|B) \) é a probabilidade de A ocorrer dado que B ocorreu.
- \( P(B|A) \) é a probabilidade de B ocorrer dado que A ocorreu.
- \( P(A) \) é a probabilidade de A ocorrer.
- \( P(B) \) é a probabilidade de B ocorrer.


O princípio fundamental do Naive Bayes é usar a probabilidade de características (ou atributos) observadas em dados para fazer previsões ou classificações. Por exemplo, se quisermos prever se um e-mail é spam ou não, poderíamos usar a frequência de certas palavras no e-mail para fazer essa previsão.

**Porque ''Naive'' (ingênuo) no nome?**

O Naive se refere a suposição fundamental do Naive Bayes, ela diz que cada característica (ou atributo) é independente das outras. Isso significa dizer que a presença (ou ausência) de uma característica não afeta a presença (ou ausência) de qualquer outra.

Essa é uma suposição muito forte e em muitas situações não reflete a realidade dos dados. Mesmo assim, o Naive Bayes em muitos casos funciona bem, ainda mais quando a dimensionalidade dos dados é alta.

Vamos supor que temos um conjunto de dados que guarde características como ''tamanho'' e ''cor'' para diferentes frutas, e nisso queremos classificar uma nova fruta.

Durante o treinamento, o Naive Bayes calcula a probabilidade de cada classe de fruta e a probabilidade de cada característica dado cada classe, então ,por exemplo, se a classe for maçã, a probabilidade da cor ser vermelha é mais alta.

Depois, quando uma nova fruta for apresentada, o método usa essas probabilidades que ele calculou no treinamento para assim calcular a probabilidade de ser cada tipo de fruta, no final ele escolhe a classe que deu a maior probabilidade.

Esse é um resumo do Naive Bayes, mais detalhes estão no notebook no repositório.






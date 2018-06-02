---
layout: simulations
categories: simulations
thumbnail: "000-thumbnail.png"
title: "Contaminação de partículas"
description: "Primeira simulação do blog, vamos começar contaminando algumas partículas?"
date: 2018-06-02
permalink: :categories/000.html
---


Simulação de contaminação de partículas, achei interessante reproduzir um ambiente de contaminação por aproximação de partículas, colocando algumas $$ N - 1 $$ partículas saudáveis e apenas uma partícula contaminada.

Vamos precisar de um ambiente para a simulação, utilizaremos um retângulo de altura/largura de acordo com o dispositivo que esteja visualizando, onde vamos adicionar algumas partículas, sendo representada por um círculo de raio $$ r $$ com coloração diferenciada entre as saudáveis (esverdeada) e contaminadas (avermelhada). A movimentação das partículas são totalmente aleatórias e a contaminação ocorre quando uma partícula contaminada encosta em uma partícula saudável, só isso!


<iframe src="https://sylviot.github.io/eng-particle-contamination" width="100%" height="300px" frameborder="0"></iframe>
<i class="fa fa-cubes"></i> <a href="https://sylviot.github.io/eng-particle-contamination" target="_blank"> Veja a simulação </a>

Um pouco de matemática, os cálculos das contaminações são realizados entre as partículas com base na fórmula de distância entre dois pontos:

$$ D_{AB} = \sqrt{ (x_B - x_A)^2 + (y_B - y_A)^2 } $$

Logo quando a soma entre os raios das partículas $$ r_A + r_B $$ forem menor que a distância entre essas partículas:

$$ D_{AB} < r_A + r_B $$

a partícula saudável se torna contaminada.

---

**O código fonte pode ser visto no repositorio:**

<i class="fa fa-github"></i> <a href="https://github.com/sylviot/eng-particle-contamination" target="_blank">  Contaminação de Partículas</a>
<br>
<i class="fa fa-cubes"></i> <a href="https://github.com/sylviot/eng-particle-contamination" target="_blank">  Veja simulação</a>


Obrigado por ler até aqui... :)
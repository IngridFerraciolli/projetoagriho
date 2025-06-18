# Projeto Agrinho
Projeto do Agrinho - Ingrid Ferraciolli

O meu jogo é bem simples. Você é uma galinha que tem que pegar os milhos e desviar dos tratores. Se você pegar milhos, você ganha um ponto, já se tocar em um trator, perde.

explicando os objetos
A "função base" do milho e do trator é o "colidiuCom()", que pega a distância entre a galinha e o milho. Se estiverem perto, o milho é coletado. Cada vez que essa função é ativada, 1 ponto é adicionado à sua pontuação.
Já para os tratores, o código detecta também a colisão com colidiuCom(). só que nesse caso, ele não dá um ponto, ele muda a variável "gameOver" para true, que te faz perder

velociade da galinha, milho e trator
A vel. dela é controlada por outra váriavel (velGalinha), que começa com um valor inical de 5. A cada 13 segundos, esse valor aumenta em 1. Logo, a velocidade da galinha também aumenta.
Os milhos e os tratores foram criados com a classe "item". Cada um desses itens tem uma velocidade inicial (BaseVel), e o tipo que varia entre "milho" e "obstáculo". A cada 10 segundos a velocidade dos dois também aumenta.


Referências: ChatGPT e Biblioteca do P5JS

#Resumo

Desenvolva, em uma linguagem de programação de sua escolha, um sistema para abrir,
exibir, manipular e salvar imagens RGB com 24 bits/pixel (8 bits/componente/pixel). Não
use bibliotecas ou funções especiais de processamento de imagens, exceto no item 6, em
que o uso de funções avançadas é livre. O sistema deve ter a seguinte funcionalidade:

- 1. Conversão RGB-YIQ-RGB (cuidado com os limites de R, G e B na volta!).

- 2. Negativo. Duas formas de aplicação devem ser testadas: em RGB (banda a banda) e
na banda Y, com posterior conversão para RGB.

- 3. Correlação m x n sobre R, G e B, com offset, e filtro especificado em um arquivo (txt)
a parte. Testar com filtros Média, Prewitt e Emboss e explicar os resultados. Para
visualização, utilize valor absoluto seguido por expansão de histograma para [0, 255].

- 4. Compare a aplicação do filtro média 21x21 com a aplicação do filtro média 21x1
seguido pela aplicação do filtro média 1x21, em termos de tempo de processamento
e resultado final, para a banda Y do YIQ.

- 5. Filtro mediana m x n sobre a banda Y do YIQ.

- 6. Reproduza o exemplo em
https://la.mathworks.com/help/images/ref/normxcorr2.html?lang=en, com as
imagens woman.png e woman_eye.png, mas aplicando a correlação normalizada
banda a banda e tomando como resultado o valor máximo das três correlações, em
cada ponto. Você pode utilizar toda a funcionalidade da linguagem de programação
de sua escolha, incluindo bibliotecas avançadas. Para visualização, utilize valor
absoluto seguido por expansão de histograma para [0, 255].

- 7. Reproduza o item 6 utilizando a função correlação desenvolvida no item 3. Para
visualização, utilize valor absoluto seguido por expansão de histograma para [0, 255].

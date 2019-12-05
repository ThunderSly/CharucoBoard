# CharucoBoard

O programa detecta os marcadores visuais a partir do dicionário pré-definido do OpenCV e a imagem.

Usando esses marcadores é possível obter os corners e suas posições.

Através dos corners e dos marcadores a câmera pode ser calibrada e consequentemente os valores da Camera Matrix e distCoeffs podem ser obtidos.

Com essas duas matrizes é possível estimar a posição com o estimatePose e obter o rvec e tvec da imagem e assim desenhar os eixos sobre o Charuco.

Em seguida são obtidos os corners da imagem original do Charuco de modo que eles possam ser utilizados para achar a matriz de homografia, juntamente com os corners do Charuco obtidos em tempo real pela webcam. 

Finalmente com a matriz de homografia em mãos pode-se usar o warpPerspective para exibir a imagem desejada sobre o Charuco.

Para ver o processo descrito acima basta abrir e rodar o /Projeto7/Projeto7.ipynb


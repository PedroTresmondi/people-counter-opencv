# people-counter-opencv
WORK IN PROGRESS


Contador de Pessoas usando OpenCV e Descritor HOG
Este script em Python utiliza a biblioteca OpenCV (Open Source Computer Vision) para realizar detecção e contagem em tempo real de pessoas em um fluxo de vídeo. Ele utiliza o método Histogram of Oriented Gradients (HOG) com um Support Vector Machine (SVM) para detecção de objetos. O script lê frames de um arquivo de vídeo (video.mp4), detecta pessoas usando um descritor HOG pré-treinado e acompanha seus movimentos cruzando uma linha especificada na tela.

Funcionalidades:
Detecção em Tempo Real: Detecta pessoas em cada frame do fluxo de vídeo usando o HOGDescriptor do OpenCV.
Rastreamento de Movimento: Acompanha pessoas cruzando uma linha específica na tela para contar entradas e saídas.
Visualização: Desenha retângulos ao redor das pessoas detectadas, sobrepondo informações de contagem no feed de vídeo e exibindo uma linha de referência.
Requisitos:
Python 3.x
Biblioteca OpenCV (cv2)
Biblioteca NumPy
Uso:
Verifique se você possui Python instalado junto com as bibliotecas necessárias.
Coloque seu arquivo de vídeo (video.mp4) no mesmo diretório que o script.
Execute o script. O vídeo começará a ser reproduzido com detecção e contagem de pessoas em tempo real.
Pressione q para sair da aplicação.
Explicação do Código:
Inicialização: Inicializa o descritor HOG e configura seu detector SVM para o detector padrão de pessoas.
Captura de Vídeo: Abre e lê frames do arquivo video.mp4.
Detecção: Aplica o detector HOG a cada frame para detectar pessoas e desenha retângulos ao redor delas.
Contagem: Acompanha pessoas cruzando uma linha horizontal pré-definida (line_y) para contar entradas (count_in) e saídas (count_out).
Visualização: Exibe o feed de vídeo com caixas de detecção, informações de contagem e uma linha de referência.
Este script demonstra uma implementação simples e eficaz de contagem de pessoas usando técnicas de visão computacional.

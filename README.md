# ReconhecimentoFacial
Projeto desenvolvido em Python usando opencv para reconhecimento facial em video e imagem.

O reconhecimento facial é umas das subáreas da Inteligência Artificial que tem como objetivo reconhecer 
faces de pessoas em imagens ou vídeos. Um exemplo são os sistemas de segurança que podem utilizar esses 
recursos para identificar se uma pessoa está ou não presente em um ambiente. 
Neste contexto é importante frisar as diferenças entre as técnicas de detecção e reconhecimento facial. 
Enquanto a primeira somente indica se uma face está presente em uma imagem, a segunda técnica tem o objetivo de 
dizer de quem é a face detectada.

Com base nisso, este projeto é focado no reconhecimento facial com o intuito de mostrar 
como reconhecer faces por imagens e pela webcam. Utilizaremos a linguagem Python e a biblioteca OpenCV, 
que é uma das mais utilizadas para processamento digital de imagens e visão computacional. 
Testes com três algoritmos disponibilizados no OpenCV, que são: Eigenfaces, Fisherfaces e LBPH. 

Avaliar a eficiência de um algoritmo de reconhecimento facial 
caso você deseje implementá-lo em ambientes comerciais.

Objetivos:
Entender os conceitos teóricos básicos sobre reconhecimento facial
Entender o funcionamento básico dos algoritmos Eigenfaces, Fisherfaces e LBPH para reconhecimento facial
Aprender a utilizar os recursos do OpenCV para reconhecer faces de imagens e pela webcam
Aprender a implementar passo a passo uma codificação para reconhecimento facial
Aprender como avaliar algoritmos de reconhecimento facial


## Installation

1)instalar o opencv no anaconda

a)criar um novo ambiente com base no python 3
b)instalar o opencv assim:
Update - 18th Jun 2019
I got this error on my Ubuntu(18.04.1 LTS) system for openCV 3.4.2, as 
the method call to cv2.imshow was failing (e.g., at the line of cv2.namedWindow(name) with error: cv2.error: 
OpenCV(3.4.2). The function is not implemented.). I am using anaconda. Just the below 2 steps helped me resolve:

```
conda remove opencv
conda install -c conda-forge opencv=4.1.0
```

If you are using pip, you can try
```
pip install opencv-contrib-python
```
# Ativar ambiente virtual obs. clicar no bash na barra de ferramentas

```
conda activate reconhecimento_facial
```
# Camera ip
camera = cv2.VideoCapture('rtsp://admin:xxxxx@192.168.0.7/live/mpeg4')

usei o O Nmap (Network Mapper) para pegar o ip da camera na minha rede:

sudo apt install nmap # Debian, Ubuntu, Linux Mint e derivados

nmap 192.168.1.*
procurar por ip que usa o protocolo rtsp

# nmap versão gráfica zenmap
sudo apt install zenmap
depois abra o zenmap pesquisando no dashboard, a versão sem root/sudo ou com root/sudo

# Próximos passos
Terminar testes com o algoritmo lbph, usar camera ip e criar app de celular
para reconhecimento facial

TestDataCollector_LBPH.py
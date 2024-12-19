# Criação de Uma Base de Dados e Treinamento da Rede YOLO

## Descrição do Desafio

Projeto de criação de uma base de dados e treinamento da rede YOLO.

Seguindo os exemplos de aula, vamos rotular uma base de dados e aplicar o treinamento com a rede YOLO.

Para essa tarefa será necessário utilizar o software [LabelMe](http://labelme.csail.mit.edu/Release3.0/) para rotular as imagens.

Também será necessário utilizar a rede YOLO, disponível em: [YOLO Darknet](https://pjreddie.com/darknet/yolo/).

Para quem preferir e não quiser rotular uma base de dados, pode usar as imagens já rotuladas do [COCO Dataset](https://cocodataset.org/#home).

E para quem estiver utilizando um computador que não consiga rodar a rede YOLO, pode utilizar o transfer learning no Colab: [Colab Transfer Learning](https://colab.research.google.com/drive/1lTGZsfMaGUpBG4inDIQwIJVW476ibXk_#scrollTo=j0t221djS1Gk).

## Requisitos

- [LabelMe](http://labelme.csail.mit.edu/Release3.0/) para rotular as imagens.
- [YOLO Darknet](https://pjreddie.com/darknet/yolo/) para o treinamento da rede.
- Alternativamente, você pode usar imagens rotuladas do [COCO Dataset](https://cocodataset.org/#home).
- Google Colab para transfer learning, se necessário: [Colab Transfer Learning](https://colab.research.google.com/drive/1lTGZsfMaGUpBG4inDIQwIJVW476ibXk_#scrollTo=j0t221djS1Gk).

## Passos para a Execução

### 1. Rotulagem das Imagens

Utilize o [LabelMe](http://labelme.csail.mit.edu/Release3.0/) para rotular suas imagens e salvar as anotações no formato JSON.

### 2. Configurar o Darknet (YOLO) no Google Colab

Clone o repositório Darknet e compile o YOLO:
```python
# Clonar o repositório darknet
!git clone https://github.com/AlexeyAB/darknet

# Ir para o diretório darknet
%cd darknet

# Compilar o darknet
!make

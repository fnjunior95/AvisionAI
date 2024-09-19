# AvisionAI - Mapeando vídeos de dança

Este projeto utiliza **FastAPI**, **MediaPipe**, **OpenCV** e **TensorFlow** para processar vídeos de dança e transformá-los em vídeos estilizados, aplicando efeitos visuais como rastreamento de movimentos e efeitos de cartoon.

## Funcionalidades

- **Upload de vídeo**: O usuário pode enviar um vídeo MP4.
- **Processamento de vídeo**: O vídeo é processado usando MediaPipe para rastreamento de poses e desenhando landmarks sobre o vídeo.
- **Download de vídeo**: O usuário pode baixar o vídeo processado.
- **Efeitos Visuais**: Aplicação opcional de efeitos como cartoonização.

## Tecnologias Usadas

- **Python 3.12**
- **FastAPI**: Framework backend.
- **MediaPipe**: Biblioteca para rastreamento de poses.
- **OpenCV**: Processamento de vídeo e imagem.
- **TensorFlow**: Utilizado como parte do MediaPipe.
- **MoviePy**: Manipulação de vídeos.
- **React**: Interface do usuário.

## Como Configurar o Projeto

### Backend

1. **Clone o repositório**:

    ```bash
    git clone [https://github.com/fnjunior95/AvisionAI.git]
    cd avisionai-backend
    ```

2. **Crie e ative o ambiente virtual**:

    ```bash
    python -m venv venv
    source venv/bin/activate  # No Windows use: venv\Scripts\activate
    ```

3. **Instale as dependências**:

    ```bash
    pip install -r requirements.txt
    ```

4. **Execute o servidor**:

    ```bash
    uvicorn main:app --reload
    ```

    O servidor rodará em `http://localhost:8000`.

### Frontend

1. **Entre na pasta do frontend**:

    ```bash
    cd avisionai-frontend
    ```

2. **Instale as dependências**:

    ```bash
    npm install
    ```

3. **Execute o frontend**:

    ```bash
    npm start
    ```

    O frontend rodará em `http://localhost:3000`.

## Como Funciona

1. O usuário faz upload de um vídeo via frontend.
2. O vídeo é enviado para o backend, onde é processado frame a frame usando MediaPipe para rastreamento de poses.
3. O vídeo processado é armazenado e o usuário pode baixá-lo com as marcações visuais de pose aplicadas.

## Melhorias Futuras

- **Processamento em tempo real**: Melhorar o tempo de processamento.
- **Aprimoramento da precisão**: Refinar o rastreamento de movimentos.
- **Suporte a outras resoluções**: Adicionar suporte para 720p e 1080p de forma automática.
- **Melhorar os efeitos visuais**: Adicionar mais efeitos opcionais.

## Dependências

Veja o arquivo [requirements.txt](requirements.txt) para a lista completa de dependências do backend.


# Aula 1 de DVC

# Como rodar este projeto

## Setup

1. Crie e ative o ambiente isolado do Conda, e instale as demais dependencias.
```
conda create --name mlops python=3.9
conda activate mlops
pip install -r requirements.txt
```

2. Solicite ao administrador do projeto o Client ID e o Client Secret Key, e faça a conexão com o google drive utilizando o dvc remote.
```
dvc remote modify --local gdrive gdrive_client_id '<Client ID>'
dvc remote modify --local gdrive gdrive_client_secret '<Client Secret Key>'
```

## Armazenando arquivos com dvc

1. Adicionando pasta com arquivo para ser commitado
```
dvc add \<Nome da Pasta>
```

2. Enviando para o repositorio remoto para armazenamento
```
dvc push
```

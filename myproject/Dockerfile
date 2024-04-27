# Use uma imagem base do Python
FROM python:latest

# Defina o diretório de trabalho como /app
WORKDIR /app

# Copie o arquivo de requisitos e instale as dependências
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

# Copie o código fonte para o diretório de trabalho
COPY . .

# Exponha a porta 8000
EXPOSE 8000

# Comando para iniciar o servidor Django
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

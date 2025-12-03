# Usa una imagen base de Python (elige una versión ligera)
FROM python:3.9-slim

# Establece el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia el archivo de requisitos al contenedor
COPY requirements.txt .

# Instala las dependencias
RUN pip install --no-cache-dir -r requirements.txt

# Copia el código de la app al contenedor
COPY app.py .

# Expone el puerto donde corre la app (Flask usa 5000 por defecto)
EXPOSE 5000

# Comando para ejecutar la app
CMD ["python", "app.py"]
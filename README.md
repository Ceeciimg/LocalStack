# Práctica 4 - LocalStack  
**Fundamentos de Computación en la Nube**

## 📌 Descripción

Esta práctica consiste en utilizar **LocalStack** para simular servicios de AWS de forma local mediante Docker Desktop con integración en WSL. Se trabajan principalmente dos servicios: **Amazon S3** y **AWS Lambda**, realizando operaciones básicas como creación de buckets, subida y descarga de archivos, y ejecución de funciones Lambda.

---

## ⚙️ Parte 1 - Preparación del entorno

1. Instalación y configuración de **Docker Desktop sobre WSL**.
2. Instalación de una distribución de Linux (Ubuntu recomendada).
3. Instalación de la extensión **LocalStack** desde Docker Desktop.
4. Ajustes en Docker Desktop:
   - Mostrar contenedores del sistema de extensiones.
   - Habilitar integración con Ubuntu desde *Resources > WSL Integration*.
5. Verificación del correcto arranque de LocalStack (capturas incluidas).
6. Ejecución del comando `aws configure` con:
   - AWS Access Key ID: `ceeciimg`
   - AWS Secret Access Key: `1234`
   - Región: `us-east-1`
   - Formato de salida: `json`

---

## 🪣 Parte 2 - Amazon S3

- Creación de dos buckets:
  - `ceeciimg-bucket-provisional`
  - `ceeciimg-bucket-definitivo`
- Subida de un archivo de texto y una imagen al bucket provisional.
- Copia de dichos archivos al bucket definitivo.
- Descarga del archivo de texto desde el bucket definitivo y muestra por terminal.
- Eliminación del bucket provisional.

---

## 🧠 Parte 3 - AWS Lambda

1. Descripción del servicio Lambda como un sistema de ejecución de funciones en la nube, que permite ejecutar código sin necesidad de aprovisionar servidores, activado por eventos.
2. Creación de `handler.py`, una función simple que devuelve un mensaje personalizado con el nombre recibido.
3. Compresión del archivo `.zip` y movimiento a la carpeta adecuada dentro de LocalStack.
4. Intento de creación de la función Lambda `ceeciimg-lambda`.
5. Intento de invocación de la función, generando el archivo `respuesta.json`.

⚠️ **Importante:**  
Después de múltiples intentos, no ha sido posible conectar con el servicio Lambda a través del puerto `4566`. El error parece estar relacionado con la limitación de la versión Community de LocalStack al utilizar Docker, como ya se indicaba en el enunciado de la práctica.  
Por tanto, el paso 6 no ha podido completarse, aunque se ha dejado constancia del error en capturas y terminal como justificación.

---

## 📷 Capturas y evidencias

Todas las capturas de pantalla y archivos relevantes han sido incluidos en este repositorio como evidencia del trabajo realizado.

---

## ✅ Estado

- [x] Parte 1 completada
- [x] Parte 2 completada
- [x] Parte 3 completada con justificación de error documentada

---

## 🧑‍💻 Autor

**Ceeciimg** – *Estudiante de DAM*  

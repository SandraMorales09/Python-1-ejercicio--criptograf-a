Proyecto de Cifrado en Python

🚀 Descripción
Este repositorio contiene ejemplos de cifrado y codificación en Python, utilizando distintos métodos clásicos y modernos.
Incluye implementaciones de:

Cifrado César

Cifrado XOR

Hashing con SHA-256

Cifrado AES (Advanced Encryption Standard)

Codificación Base64

Generación de contraseñas aleatorias

📂 Contenido del repositorio
Código
├── cifrado_cesar.py        # Implementación del cifrado y descifrado César
├── cifrado_xor.py          # Implementación del cifrado XOR
├── hashing.py              # Generación de hash SHA-256
├── cifrado_aes.py          # Cifrado y descifrado con AES
├── base64_encode.py        # Codificación en Base64
├── password_generator.py   # Generador de contraseñas seguras
└── README.md               # Documentación del proyecto
⚙️ Requisitos
Python 3.8 o superior

Librerías estándar de Python (hashlib, base64, random, string)

Librería externa cryptography para AES:

bash
pip install cryptography
🛠️ Ejemplos de uso
🔑 Cifrado César
python
mensaje = "Hola Mundo"
clave = 3
mensaje_cifrado = cifrar_cesar(mensaje, clave)
mensaje_descifrado = descifrar_cesar(mensaje_cifrado, clave)

print("Mensaje cifrado:", mensaje_cifrado)
print("Mensaje descifrado:", mensaje_descifrado)
⚡ Cifrado XOR
python
mensaje = "Python Rocks"
clave = 42
mensaje_cifrado = cifrar_xor(mensaje, clave)
mensaje_descifrado = cifrar_xor(mensaje_cifrado, clave)

print("Mensaje cifrado:", mensaje_cifrado)
print("Mensaje descifrado:", mensaje_descifrado)
🧩 Hashing con SHA-256
python
mensaje = "Este es un mensaje importante"
hash_generado = generar_hash(mensaje)

print("Mensaje:", mensaje)
print("Hash SHA256:", hash_generado)
🔒 Cifrado AES
python
clave = os.urandom(32)  # Clave de 256 bits
mensaje = "Hola AES!"
iv, mensaje_cifrado = cifrar_aes(mensaje, clave)
mensaje_descifrado = descifrar_aes(mensaje_cifrado, clave, iv)

print("Mensaje cifrado:", mensaje_cifrado)
print("Mensaje descifrado:", mensaje_descifrado)
📦 Codificación Base64
python
print(codificar_base64("Hola Mundo"))
🔐 Generador de contraseñas
python
print(generar_contraseña(12))
📖 Consultas de práctica
Probar distintos valores de clave en el Cifrado César.

Usar diferentes longitudes de clave en AES (128, 192, 256 bits).

Generar hashes de varios mensajes y verificar su integridad.

Crear contraseñas seguras de 8, 12 y 16 caracteres.

🤝 Contribución
Haz un fork del repositorio.

Crea una rama para tus cambios:

bash
git checkout -b mi-feature

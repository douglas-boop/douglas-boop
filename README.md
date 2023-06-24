- 👋 Hi, I’m @douglas-boob
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
douglas-boop/douglas-boop is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
from PIL import Image

# Sequência de números fornecida
sequence = [0, 0, 0, 46, 46, 46, 46, 113, 117, 114, 46, 99, 111, 109, 47, 32, 97, 47, 32, 113, 50, 112, 48, 116, 106, 97]

# Converter a sequência em uma string
sequence_str = ''.join(chr(num) for num in sequence)

# Salvar a string como imagem
with open('image.jpg', 'wb') as f:
    f.write(sequence_str.encode())

# Abrir e exibir a imagem
image = Image.open('image.jpg')
image.show()

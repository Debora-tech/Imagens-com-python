# Imagens-com-python
from PIL import Image, ImageFilter

def open_image(file_path):
    """Abre uma imagem de um arquivo e retorna o objeto Image."""
    return Image.open(file_path)

def save_image(image, output_path):
    """Salva uma imagem no diretório especificado."""
    image.save(output_path)

def apply_blur(image):
    """Aplica um filtro de desfoque na imagem."""
    return image.filter(ImageFilter.BLUR)

def resize_image(image, size):
    """Redimensiona a imagem para o tamanho especificado."""
    return image.resize(size)

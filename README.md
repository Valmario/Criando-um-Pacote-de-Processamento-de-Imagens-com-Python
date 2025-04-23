# 📦 Criando um Pacote de Processamento de Imagens com Python

![GitHub License](https://img.shields.io/github/license/Valmario/Criando-um-Pacote-de-Processamento-de-Imagens-com-Python?style=flat-square)
![GitHub Last Commit](https://img.shields.io/github/last-commit/Valmario/Criando-um-Pacote-de-Processamento-de-Imagens-com-Python?style=flat-square)
![GitHub Language Count](https://img.shields.io/github/languages/count/Valmario/Criando-um-Pacote-de-Processamento-de-Imagens-com-Python?style=flat-square)
![GitHub Top Language](https://img.shields.io/github/languages/top/Valmario/Criando-um-Pacote-de-Processamento-de-Imagens-com-Python?style=flat-square)
![Python Version](https://img.shields.io/badge/python-3.8%2B-blue?style=flat-square)
![Build](https://img.shields.io/badge/build-passing-brightgreen?style=flat-square)

Neste projeto você aprenderá a criar seu **primeiro pacote de processamento de imagens em Python** e publicá-lo no **PyPI** para reutilização e compartilhamento. O exemplo prático irá te guiar na construção do pacote, estruturação do projeto, publicação e testes locais e na nuvem.

---

## 🧠 O que você vai aprender?

- Criar e organizar um pacote Python do zero
- Utilizar `setuptools`, `twine` e `wheel`
- Publicar pacotes no TestPyPI e no PyPI oficial
- Utilizar funções úteis para manipulação de imagens
- Documentar, versionar e empacotar seu código

---

## 🛠 Tecnologias Utilizadas

- **Python** 
- **Git**
- **Setuptools**
- **Twine**
- **Pillow / OpenCV (dependendo da implementação)**

---

## ✅ Requisitos Básicos

- Python instalado (`>=3.6`)
- Git instalado
- Conta no [TestPyPI](https://test.pypi.org/account/register/) e [PyPI](https://pypi.org/account/register/)
- Projeto Python com arquivos estruturados

---

## ⚙️ Estrutura do Projeto

```
project_name/
│
├── package_name/
│   ├── __init__.py
│   ├── module1.py
│   └── module2.py
│
├── tests/
│   ├── __init__.py
│   └── test_module1.py
│
├── setup.py
├── README.md
├── requirements.txt
└── LICENSE
```

---

## 🚀 Criando o Projeto

1. Faça o fork do template base
2. Adicione o conteúdo dos módulos e funções
3. Configure o `setup.py` corretamente
4. Atualize o `requirements.txt` com suas dependências
5. Escreva um `README.md` completo (como este 😉)

---

## 📦 Gerando as Distribuições

Instale os pacotes necessários:

```bash
python -m pip install --upgrade pip
python -m pip install --user setuptools wheel twine
```

Gere a distribuição:

```bash
python setup.py sdist bdist_wheel
```

---

## ☁️ Publicando o Pacote

### 📤 No Test PyPI

```bash
python -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
```

Instale e teste o pacote com:

```bash
pip install --index-url https://test.pypi.org/simple/ image-processing
```

### 📤 No PyPI oficial

```bash
python -m twine upload dist/*
```

Instale normalmente com:

```bash
pip install image-processing
```

---

## 🧪 Exemplo de Uso

```python
from package_name.module1 import resize_image
resize_image("input.jpg", "output.jpg", size=(256, 256))
```

---

## 📚 Funcionalidades

### Processing

- Histogram Matching
- Structural Similarity
- Resize de Imagens

### Utils

- Leitura e salvamento de imagens
- Plotagem de imagens e resultados
- Visualização de histogramas

---

## 🔗 Links Úteis

- 📘 [Documentação do Setuptools](https://setuptools.readthedocs.io/en/latest/setuptools.html)
- ✅ [Testes com PyTest](https://docs.pytest.org/en/latest/)
- 🧪 [Uso do Tox](https://tox.readthedocs.io/en/latest/)
- 🧱 [Template base no GitHub](https://github.com/tiemi/package-template)
- 🧪 [Test PyPI](https://test.pypi.org/)
- 🌍 [PyPI Oficial](https://pypi.org/)

---

![Banner](https://assets.dio.me/IwGGaOEYVw9pPUMVGEaqp7eKn1gV22wDOHmmAmI0zDY/f:webp/h:221/q:80/L3RyYWNrcy9jb3Zlci83OWZiNzhkZC0xNTQ3LTQ0N2YtYTNkOC04ZGQwMWU1YWMzNTEucG5n)

---

## 👨‍💻 Projeto desenvolvido no

[**Bootcamp Suzano - Python Developer**](https://www.dio.me/bootcamp/suzano-python-developer), promovido por [**DIO**](https://www.dio.me/)

---

## ✨ Autor

- [Valmário](https://github.com/Valmario)

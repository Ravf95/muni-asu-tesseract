Pruebas con tessaract para la extracción de 
datos sobre el pdf seleccionable resultante.

### Dataset
#
https://data.controlciudadanopy.org/municipalidad/

### Formato: documentos a ser analizados
#
downloadDate(%y-%MM-%dd)_hashDocument_(%Mon_%y).pdf

### Dependencias
#
- pdfseparate
- pdftoppm
- img2pdf
- ocrmypdf
- pdftotext
- tesseract

### TODO
#
- Reducir dpi y analizar resultados
- Utilizar liberias con control de stdout y stderr para automatizar el proceso de ocr

    Python 3: comando/wrapper
   - pdfseparate:     subprocess call
   - pdftoppm:        subprocess call / https://pypi.org/project/pdf2image/
   - img2pdf:         subprocess call / https://pypi.org/project/img2pdf/
   - ocrmypdf:        subprocess call / https://pypi.org/project/ocrmypdf/
   - pdftotext:       subprocess call / https://pypi.org/project/pdftotext/
   - tabula:          subprocess call / https://pypi.org/project/tabula-py/


- Evaluar resultados sobre el pdf seleccionable con:
    - https://github.com/pdfminer/pdfminer.six
    - https://github.com/camelot-dev/camelot

- Parsear resultados por página



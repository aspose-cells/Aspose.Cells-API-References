---
title: Font clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 650
url: /es/python-net/aspose.cells/font/
is_root: false
---
##  Font clase
Encapsula el objeto de fuente utilizado en una hoja de cálculo.



El tipo Font expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [charset](/cells/es/python-net/aspose.cells/font/charset) | Representar el conjunto de caracteres.|
| [is_italic](/cells/es/python-net/aspose.cells/font/is_italic) | Obtiene o establece un valor que indica si la fuente está en cursiva.|
| [is_bold](/cells/es/python-net/aspose.cells/font/is_bold) |Obtiene o establece un valor que indica si la fuente está en negrita.|
| [caps_type](/cells/es/python-net/aspose.cells/font/caps_type) | Obtiene y establece el tipo de mayúsculas de texto.|
| [strike_type](/cells/es/python-net/aspose.cells/font/strike_type) | Obtiene el tipo de aviso del texto.|
| [is_strikeout](/cells/es/python-net/aspose.cells/font/is_strikeout) | Obtiene o establece un valor que indica si la fuente está tachada.|
| [script_offset](/cells/es/python-net/aspose.cells/font/script_offset) | Obtiene y establece el desplazamiento del script, en unidades de porcentaje|
| [is_superscript](/cells/es/python-net/aspose.cells/font/is_superscript) | Obtiene o establece un valor que indica si la fuente es superscript.|
| [is_subscript](/cells/es/python-net/aspose.cells/font/is_subscript) | Obtiene o establece un valor que indica si la fuente es un subíndice.|
| [underline](/cells/es/python-net/aspose.cells/font/underline) | Obtiene o establece el tipo de subrayado de la fuente.|
| [name](/cells/es/python-net/aspose.cells/font/name) | Obtiene o establece el nombre de [Font](/cells/es/python-net/aspose.cells/font).|
| [double_size](/cells/es/python-net/aspose.cells/font/double_size) | Obtiene y establece el tamaño doble de la fuente.|
| [size](/cells/es/python-net/aspose.cells/font/size) | Obtiene o establece el tamaño de la fuente.|
| [theme_color](/cells/es/python-net/aspose.cells/font/theme_color) | Obtiene y establece el color del tema.|
| [color](/cells/es/python-net/aspose.cells/font/color) | Obtiene o establece el Color de la fuente.|
| [argb_color](/cells/es/python-net/aspose.cells/font/argb_color) | Obtiene y establece el color con un valor ARGB de 32 bits.|
| [is_normalize_heights](/cells/es/python-net/aspose.cells/font/is_normalize_heights) | Indica si la normalización de altura que se va a aplicar al texto se ejecuta.|
| [scheme_type](/cells/es/python-net/aspose.cells/font/scheme_type) | Obtiene y establece el tipo de esquema de la fuente.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [equals(font)](/cells/es/python-net/aspose.cells/font/equals/#Font) | Comprueba si dos fuentes son iguales.|



###  Ejemplos

```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Accessing the "A1" cell from the worksheet
cell = worksheet.cells.get("A1")
# Adding some value to the "A1" cell
cell.put_value("Hello Aspose!")
font = cell.get_style().font
# Setting the font name to "Times New Roman"
font.name = "Times New Roman"
# Setting font size to 14
font.size = 14
# setting font color as Red
font.color = Color.red
# Saving the Excel file
workbook.save(r"dest.xls")

```

###  Ver también
* módulo [aspose.cells](..)
* clase [Font](/cells/es/python-net/aspose.cells/font)

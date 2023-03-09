---
title: Hyperlink clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 790
url: /es/python-net/aspose.cells/hyperlink/
is_root: false
---
##  Hyperlink clase
Encapsula el objeto que representa un hipervínculo.



El tipo Hyperlink expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [address](/cells/es/python-net/aspose.cells/hyperlink/address) | Representa la dirección de un hipervínculo.|
| [text_to_display](/cells/es/python-net/aspose.cells/hyperlink/text_to_display) | Representa el texto que se mostrará para el hipervínculo especificado.|
| [area](/cells/es/python-net/aspose.cells/hyperlink/area) | Obtiene el rango de hipervínculos.|
| [screen_tip](/cells/es/python-net/aspose.cells/hyperlink/screen_tip) | Devuelve o establece el texto de información en pantalla para el hipervínculo especificado.|
| [link_type](/cells/es/python-net/aspose.cells/hyperlink/link_type) | Obtiene el tipo de vínculo.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [delete()](/cells/es/python-net/aspose.cells/hyperlink/delete/#) | Elimina este hipervínculo|



###  Ejemplos

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Workbook object
workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Adding a hyperlink to a URL at "A1" cell
index = worksheet.hyperlinks.add("A1", 1, 1, "http://www.aspose.com")
# Getting a Hyperlink by index.
hyperlink = worksheet.hyperlinks[index]
# Setting display text of this hyperlink.
hyperlink.text_to_display = "Aspose"
# Saving the Excel file
workbook.save("book1.xls")

```

###  Ver también
* módulo [aspose.cells](..)

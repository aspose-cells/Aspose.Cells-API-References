---
title: ContentTypeProperty clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells.properties/contenttypeproperty/
is_root: false
---
##  ContentTypeProperty clase
Representa información del identificador.



El tipo ContentTypeProperty expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [name](/cells/es/python-net/aspose.cells.properties/contenttypeproperty/name) | Devuelve o establece el nombre del objeto.|
| [value](/cells/es/python-net/aspose.cells.properties/contenttypeproperty/value) | Devuelve o establece el valor de la propiedad de tipo de contenido.|
| [type](/cells/es/python-net/aspose.cells.properties/contenttypeproperty/type) | Obtiene y establece el tipo de la propiedad.|
| [is_nillable](/cells/es/python-net/aspose.cells.properties/contenttypeproperty/is_nillable) | Indica si el valor podría estar vacío.|



###  Ejemplos

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Add a new property.
workbook.content_type_properties.add("Admin", "Aspose", "text")
# Save the Excel file
workbook.save("book1.xlsm")

```

###  Ver también
* módulo [aspose.cells.properties](..)

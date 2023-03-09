---
title: ExternalLinkCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 570
url: /es/python-net/aspose.cells/externallinkcollection/
is_root: false
---
##  ExternalLinkCollection clase
Representa una colección de enlaces externos en un libro de trabajo.



El tipo ExternalLinkCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [count](/cells/es/python-net/aspose.cells/externallinkcollection/count) | Obtiene el número de elementos realmente contenidos en la colección.|



Obtiene el elemento [ExternalLink](/cells/es/python-net/aspose.cells/externallink) en el índice especificado.
###  indexador
| Nombre| Descripción|
| :- | :- |
| [index] | El índice de base cero del elemento.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add(file_name, sheet_names)](/cells/es/python-net/aspose.cells/externallinkcollection/add/#str-list) | Agrega un enlace externo.|
| [add(directory_type, file_name, sheet_names)](/cells/es/python-net/aspose.cells/externallinkcollection/add/#DirectoryType-str-list) | Añadir un enlace externo.|
| [clear()](/cells/es/python-net/aspose.cells/externallinkcollection/clear/#) | Elimina todos los enlaces externos.|
| [clear(update_references_as_local)](/cells/es/python-net/aspose.cells/externallinkcollection/clear/#bool) | Elimina todos los enlaces externos.|
| [remove_at(index)](/cells/es/python-net/aspose.cells/externallinkcollection/remove_at/#int) | Elimina el vínculo externo especificado del libro de trabajo.|
| [remove_at(index, update_references_as_local)](/cells/es/python-net/aspose.cells/externallinkcollection/remove_at/#int-bool) | Elimina el vínculo externo especificado del libro de trabajo.|



###  Ejemplos

```python
from aspose.cells import Workbook

# Open a file with external links
workbook = Workbook("book1.xls")
# Change external link data source
workbook.worksheets.external_links[0].data_source = "d:\\link.xls"

```

###  Ver también
* módulo [aspose.cells](..)
* clase [ExternalLink](/cells/es/python-net/aspose.cells/externallink)

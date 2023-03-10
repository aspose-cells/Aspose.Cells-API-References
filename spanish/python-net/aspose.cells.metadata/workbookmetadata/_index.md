---
title: WorkbookMetadata clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells.metadata/workbookmetadata/
is_root: false
---
##  WorkbookMetadata clase
Representa los metadatos.



El tipo WorkbookMetadata expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [WorkbookMetadata(file_name, options)](/cells/es/python-net/aspose.cells.metadata/workbookmetadata/__init__/#str-MetadataOptions) | Cree el objeto de metadatos.|
| [WorkbookMetadata(stream, options)](/cells/es/python-net/aspose.cells.metadata/workbookmetadata/__init__/#io.RawIOBase-MetadataOptions) | Cree el objeto de metadatos.|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [options](/cells/es/python-net/aspose.cells.metadata/workbookmetadata/options) | Obtiene las opciones de los metadatos.|
| [built_in_document_properties](/cells/es/python-net/aspose.cells.metadata/workbookmetadata/built_in_document_properties) |Devuelve una colección [DocumentProperty](/cells/es/python-net/aspose.cells.properties/documentproperty) que representa todas las propiedades de documento integradas de la hoja de cálculo.|
| [custom_document_properties](/cells/es/python-net/aspose.cells.metadata/workbookmetadata/custom_document_properties) | Devuelve una colección [DocumentProperty](/cells/es/python-net/aspose.cells.properties/documentproperty) que representa todas las propiedades del documento personalizado de la hoja de cálculo.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [save(file_name)](/cells/es/python-net/aspose.cells.metadata/workbookmetadata/save/#str) | Guarde los metadatos modificados en el archivo.|
| [save(stream)](/cells/es/python-net/aspose.cells.metadata/workbookmetadata/save/#io.RawIOBase) | Guarde los metadatos modificados en la secuencia.|



###  Ejemplo

El siguiente ejemplo crea un WorkbookMetadata.

```python
from aspose.cells.metadata import MetadataOptions, MetadataType, WorkbookMetadata

options = MetadataOptions(MetadataType.DOCUMENT_PROPERTIES)
meta = WorkbookMetadata("book1.xlsx", options)
meta.custom_document_properties.add("test", "test")
meta.save("book2.xlsx")

```

###  Ver también
* módulo [aspose.cells.metadata](..)
* clase [DocumentProperty](/cells/es/python-net/aspose.cells.properties/documentproperty)

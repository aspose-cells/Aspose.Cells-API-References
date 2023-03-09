---
title: export_object método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/iexportobjectlistener/export_object/
is_root: false
---
##  export_object(e) {#ExportObjectEvent}
Exportar un objeto.


###  Devoluciones

La información sobre el resultado de la exportación del objeto.

* Para exportar objetos al exportar el libro de trabajo al formato HTML,
el resultado es una cadena URL para acceder a la imagen guardada desde el archivo html que contiene este objeto exportado.


```python
def export_object(self, e):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| e | [ExportObjectEvent](/cells/es/python-net/aspose.cells/exportobjectevent) | El evento se activa cuando es necesario exportar un objeto.|



###  Ver también
* módulo [aspose.cells](../../)
* clase [IExportObjectListener](/cells/es/python-net/aspose.cells/iexportobjectlistener)

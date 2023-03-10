---
title: refer_to_sheet_with_same_name propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 90
url: /es/python-net/aspose.cells/copyoptions/refer_to_sheet_with_same_name/
is_root: false
---
##  refer_to_sheet_with_same_name propiedad

Al copiar una hoja de trabajo a otro libro de trabajo y la hoja de trabajo contiene las fórmulas que se refieren a otras hojas de trabajo en MS Excel,
las fórmulas copiadas deben hacer referencia al libro de trabajo de origen.
Pero a veces hemos copiado otras hojas de trabajo y esperamos que las fórmulas copiadas se refieran a otras hojas de trabajo con el nombre en el mismo libro de trabajo,
establezca esta propiedad como verdadera.

###  Observaciones

El valor por defecto es verdadero.
###  Definición:
```python
@property
def refer_to_sheet_with_same_name(self):
    ...
@refer_to_sheet_with_same_name.setter
def refer_to_sheet_with_same_name(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [CopyOptions](/cells/es/python-net/aspose.cells/copyoptions)

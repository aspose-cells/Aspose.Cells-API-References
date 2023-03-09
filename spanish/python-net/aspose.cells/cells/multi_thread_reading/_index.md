---
title: multi_thread_reading propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1200
url: /es/python-net/aspose.cells/cells/multi_thread_reading/
is_root: false
---
##  multi_thread_reading propiedad

Obtiene o establece si el modelo de datos de las celdas debe admitir la lectura de subprocesos múltiples.
El valor predeterminado de esta propiedad es falso.

###  Observaciones

Si hay varios subprocesos para leer objetos Row/Cell en esta colección al mismo tiempo,
esta propiedad debe establecerse como verdadera, de lo contrario, se pueden producir resultados inesperados.
La compatibilidad con la lectura de subprocesos múltiples puede degradar el rendimiento para acceder a los objetos Row/Cell de esta colección.
Tenga en cuenta que algunas características no pueden admitir la lectura de subprocesos múltiples,
como valores de formato (por [Cell.string_value](/cells/es/python-net/aspose.cells/cell#string_value), [Cell.display_string_value](/cells/es/python-net/aspose.cells/cell#display_string_value), .etc.).
Por lo tanto, incluso con esta propiedad configurada como verdadera, esas API aún pueden dar un resultado inesperado para la lectura de subprocesos múltiples.
###  Definición:
```python
@property
def multi_thread_reading(self):
    ...
@multi_thread_reading.setter
def multi_thread_reading(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [Cells](/cells/es/python-net/aspose.cells/cells)

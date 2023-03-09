---
title: start_access_cache método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 380
url: /es/python-net/aspose.cells/workbook/start_access_cache/
is_root: false
---
##  start_access_cache(opts) {#AccessCacheOptions}
Inicia la sesión que utiliza cachés para acceder a los datos.



```python
def start_access_cache(self, opts):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| opts | [AccessCacheOptions](/cells/es/python-net/aspose.cells/accesscacheoptions) | opciones de acceso a datos|
###  Observaciones

Si el caché de acceso a datos especificado requiere que algunos modelos de datos en la hoja de trabajo sean de "solo lectura",
entonces los modelos de datos correspondientes en cada hoja de trabajo en este libro de trabajo se tomarán como "solo lectura"
y el usuario no debe cambiar ninguno de ellos.


Después de finalizar el acceso a los datos, [Workbook.close_access_cache(opts)](/cells/es/python-net/aspose.cells/workbook/close_access_cache) debería
ser invocado con las mismas opciones para borrar todos los cachés y recuperar el modo de acceso normal.


###  Ver también
* módulo [aspose.cells](../../)
* clase [Workbook](/cells/es/python-net/aspose.cells/workbook)

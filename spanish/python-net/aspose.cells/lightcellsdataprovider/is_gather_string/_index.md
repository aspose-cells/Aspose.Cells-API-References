---
title: is_gather_string método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/
is_root: false
---
##  is_gather_string() {#}
Comprueba si el valor de cadena actual de la celda debe recopilarse en un grupo global.


###  Devoluciones

true si el valor de la cadena debe recopilarse en un grupo global para el archivo resultante.


```python
def is_gather_string(self):
    ...
```


###  Observaciones

La recopilación de valores de cadena se aprovechará solo cuando haya muchos valores de cadena duplicados para las celdas proporcionadas por esta implementación.
En esta situación, la recopilación de cadenas ahorrará mucha memoria y generará un archivo resultante más pequeño.
Si hay muchos valores de cadena para las celdas proporcionadas por LightCellsDataProvider pero pocos de ellos son iguales,
recopilar cadenas costará más memoria y tiempo y no tiene ninguna ventaja para el archivo resultante.


###  Ver también
* módulo [aspose.cells](../../)
* clase [LightCellsDataProvider](/cells/es/python-net/aspose.cells/lightcellsdataprovider)

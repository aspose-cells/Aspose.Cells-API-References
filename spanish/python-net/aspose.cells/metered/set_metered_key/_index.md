---
title: set_metered_key método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells/metered/set_metered_key/
is_root: false
---
##  set_metered_key(public_key, private_key) {#str-str}
Establece la clave pública y privada medidas.
Si compra una licencia medida, cuando inicie la solicitud, debe llamar a este API, normalmente, esto es suficiente. Sin embargo, si siempre falla en cargar los datos de consumo y excede las 24 horas, la licencia se establecerá en estado de evaluación, para evitar tal caso, debe verificar periódicamente el estado de la licencia, si es el estado de evaluación, llame nuevamente a este API.



```python
def set_metered_key(self, public_key, private_key):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| public_key | str | Llave pública|
| private_key | str | llave privada|



###  Ver también
* módulo [aspose.cells](../../)
* clase [Metered](/cells/es/python-net/aspose.cells/metered)

---
title: Metered clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1050
url: /es/python-net/aspose.cells/metered/
is_root: false
---
##  Metered clase
Proporciona métodos para configurar la clave medida.



El tipo Metered expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [Metered()](/cells/es/python-net/aspose.cells/metered/__init__/#) | Inicializa una nueva instancia de esta clase.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [set_metered_key(public_key, private_key)](/cells/es/python-net/aspose.cells/metered/set_metered_key/#str-str) | Establece la clave pública y privada medida.<br/>Si compra una licencia medida, cuando inicie la solicitud, debe llamar a este API, normalmente, esto es suficiente. Sin embargo, si siempre falla en cargar los datos de consumo y excede las 24 horas, la licencia se establecerá en estado de evaluación, para evitar tal caso, debe verificar periódicamente el estado de la licencia, si es el estado de evaluación, llame nuevamente a este API.|
| [get_consumption_quantity()](/cells/es/python-net/aspose.cells/metered/get_consumption_quantity/#) | Obtiene el tamaño del archivo de consumo|
| [get_consumption_credit()](/cells/es/python-net/aspose.cells/metered/get_consumption_credit/#) | Obtiene crédito de consumo|



###  Ejemplo

En este ejemplo, se intentará establecer una clave pública y privada medidas


```python
from aspose.cells import Metered

matered = Metered()
matered.set_metered_key("PublicKey", "PrivateKey")

```

###  Ver también
* módulo [aspose.cells](..)

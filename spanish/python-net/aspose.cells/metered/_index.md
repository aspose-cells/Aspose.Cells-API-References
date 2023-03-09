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
Proporciona métodos para establecer claves medidas.



El tipo Metered expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [Metered()](/cells/es/python-net/aspose.cells/metered/__init__/#) | Inicializa una nueva instancia de esta clase.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [set_metered_key(public_key, private_key)](/cells/es/python-net/aspose.cells/metered/set_metered_key/#str-str) | Establece claves públicas y privadas medidas.<br/>Si compra una licencia con medidor, cuando inicie la solicitud, debe llamar a este API, normalmente, esto es suficiente. Debe verificar regularmente el estado de la licencia, si es un estado de evaluación, llame a este API nuevamente.|
| [get_consumption_quantity()](/cells/es/python-net/aspose.cells/metered/get_consumption_quantity/#) | Obtiene el tamaño del archivo de consumo|
| [get_consumption_credit()](/cells/es/python-net/aspose.cells/metered/get_consumption_credit/#) | Obtiene crédito de consumo|



###  Ejemplos

En este ejemplo, se intentará establecer claves públicas y privadas medidas


```python
from aspose.cells import Metered

matered = Metered()
matered.set_metered_key("PublicKey", "PrivateKey")

```

###  Ver también
* módulo [aspose.cells](..)

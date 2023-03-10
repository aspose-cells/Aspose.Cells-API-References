---
title: License clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 980
url: /es/python-net/aspose.cells/license/
is_root: false
---
##  License clase
Proporciona métodos para licenciar el componente.



El tipo License expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [License()](/cells/es/python-net/aspose.cells/license/__init__/#) | Inicializa una nueva instancia de esta clase.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [set_license(license_name)](/cells/es/python-net/aspose.cells/license/set_license/#str) | Licencia el componente.|
| [set_license(stream)](/cells/es/python-net/aspose.cells/license/set_license/#io.RawIOBase) | Licencia el componente.|



###  Ejemplo

En este ejemplo, se intentará encontrar un archivo de licencia llamado MyLicense.lic
 en la carpeta que contiene


el componente, en la carpeta que contiene el ensamblaje de llamada,
en la carpeta del ensamblado de entrada y luego en los recursos incrustados del ensamblado que llama.

```python
from aspose.cells import License

license = License()
license.set_license("MyLicense.lic")

```

###  Ver también
* módulo [aspose.cells](..)

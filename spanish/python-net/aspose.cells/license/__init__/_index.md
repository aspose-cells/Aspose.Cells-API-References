---
title: License constructor
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 10
url: /es/python-net/aspose.cells/license/__init__/
is_root: false
---
##  License() {#}
Inicializa una nueva instancia de esta clase.



```python
def __init__(self):
    ...
```



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
* módulo [aspose.cells](../../)
* clase [License](/cells/es/python-net/aspose.cells/license)

---
title: classe License
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 980
url: /it/python-net/aspose.cells/license/
is_root: false
---
##  classe License
Fornisce i metodi per concedere in licenza il componente.



Il tipo License espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [License()](/cells/it/python-net/aspose.cells/license/__init__/#) | Inizializza una nuova istanza di questa classe.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [set_license(license_name)](/cells/it/python-net/aspose.cells/license/set_license/#str) | Concede in licenza il componente.|
| [set_license(stream)](/cells/it/python-net/aspose.cells/license/set_license/#io.RawIOBase) | Concede in licenza il componente.|



###  Esempio

In questo esempio, verrà effettuato un tentativo di trovare un file di licenza denominato MyLicense.lic
 nella cartella che contiene


il componente, nella cartella che contiene l'assembly chiamante,
nella cartella dell'assembly di ingresso e quindi nelle risorse incorporate dell'assembly chiamante.

```python
from aspose.cells import License

license = License()
license.set_license("MyLicense.lic")

```

###  Guarda anche
* modulo [aspose.cells](..)

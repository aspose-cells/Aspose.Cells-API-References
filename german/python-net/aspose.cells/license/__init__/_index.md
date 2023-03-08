---
title: License Konstrukteur
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 10
url: /de/python-net/aspose.cells/license/__init__/
is_root: false
---
##  License() {#}
Initialisiert eine neue Instanz dieser Klasse.



```python
def __init__(self):
    ...
```



###  Beispiel

In diesem Beispiel wird versucht, eine Lizenzdatei namens MyLicense.lic zu finden
 in dem Ordner, der enthält


die Komponente in dem Ordner, der die aufrufende Assembly enthält,
im Ordner der Eintragsassembly und dann in den eingebetteten Ressourcen der aufrufenden Assembly.

```python
from aspose.cells import License

license = License()
license.set_license("MyLicense.lic")

```



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [License](/cells/de/python-net/aspose.cells/license)

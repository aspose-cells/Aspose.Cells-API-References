---
title: culture_custom Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 170
url: /de/python-net/aspose.cells/style/culture_custom/
is_root: false
---
##  culture_custom Eigentum

Ruft die kulturabhängige Musterzeichenfolge für das Zahlenformat ab und legt sie fest.
Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben.
Wenn das Zahlenformat eingebaut ist, wird die Musterzeichenfolge zurückgegeben, die der eingebauten Zahl entspricht.

###  Bemerkungen

Für das integrierte Zahlenformat sind sowohl der Musterinhalt (z. B. ein integriertes Datumsformat ist „m/d/y“ für einige Gebietsschemata,
aber für einige andere Gebietsschemas wird es "d/m/y") und der Formatbezeichner (wie z.
einige Gebietsschemas verwenden andere Zeichen als „y“, um den Jahresteil für die Datumsformatierung darzustellen)
sind kulturabhängig;
Für vom Benutzer angegebene benutzerdefinierte Formate werden nur Formatbezeichner entsprechend der Kultur geändert,
andere Teile des Formatierungsmusters werden nicht geändert.
###  Definition:
```python
@property
def culture_custom(self):
    ...
@culture_custom.setter
def culture_custom(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Style](/cells/de/python-net/aspose.cells/style)

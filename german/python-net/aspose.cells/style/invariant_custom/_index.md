---
title: invariant_custom Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 260
url: /de/python-net/aspose.cells/style/invariant_custom/
is_root: false
---
##  invariant_custom Eigentum

Ruft die kulturunabhängige Musterzeichenfolge für das Zahlenformat ab.
Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben.
Wenn das Zahlenformat eingebaut ist, wird die Musterzeichenfolge zurückgegeben, die der eingebauten Zahl entspricht.

###  Bemerkungen

Für integrierte Zahlenformate ist der zurückgegebene Musterinhalt immer noch kulturabhängig,
Beispielsweise gibt es für einige Gebietsschemas "m/d/y" und für einige andere Gebietsschemas "d/m/y" zurück.
Der Unterschied zu [Style.culture_custom](/cells/de/python-net/aspose.cells/style#culture_custom) ist (das bedeutet auch kulturunabhängig):
die Formatbezeichner und Trennzeichen werden standardmäßig beibehalten, z. B. '/' wird immer als Datum/Uhrzeit-Trennzeichen verwendet
und "y" wird immer als "year"-Teil verwendet, egal welche anderen Sonderzeichen für die spezifische Locale verwendet werden.
###  Definition:
```python
@property
def invariant_custom(self):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Style](/cells/de/python-net/aspose.cells/style)

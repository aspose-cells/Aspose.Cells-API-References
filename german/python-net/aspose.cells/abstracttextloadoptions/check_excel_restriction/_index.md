---
title: check_excel_restriction Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 70
url: /de/python-net/aspose.cells/abstracttextloadoptions/check_excel_restriction/
is_root: false
---
##  check_excel_restriction Eigentum

Ob die Einschränkung der Excel-Datei überprüft wird, wenn der Benutzer zellenbezogene Objekte ändert.
Beispielsweise erlaubt Excel keine Eingabe von Zeichenfolgenwerten, die länger als 32 KB sind.
Wenn Sie einen Wert eingeben, der länger als 32 KB ist, wie z. B. Cell.PutValue(string), erhalten Sie eine Ausnahme, wenn diese Eigenschaft wahr ist.
Wenn diese Eigenschaft "false" ist, akzeptieren wir Ihren Eingabe-String-Wert als Wert der Zelle, damit dies später möglich ist
bei anderen Dateiformaten wie CSV können Sie den kompletten Stringwert ausgeben.
Wenn Sie jedoch einen solchen Wert festgelegt haben, der für das Excel-Dateiformat ungültig ist,
Sie sollten die Arbeitsmappe später nicht als Excel-Dateiformat speichern. Andernfalls kann es zu unerwarteten Fehlern in der generierten Excel-Datei kommen.
###  Definition:
```python
@property
def check_excel_restriction(self):
    ...
@check_excel_restriction.setter
def check_excel_restriction(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [AbstractTextLoadOptions](/cells/de/python-net/aspose.cells/abstracttextloadoptions)

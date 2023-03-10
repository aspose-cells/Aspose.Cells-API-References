---
title: protect Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 180
url: /de/python-net/aspose.cells/worksheet/protect/
is_root: false
---
##  protect(type) {#ProtectionType}
Schützt Arbeitsblatt.



```python
def protect(self, type):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| type | [ProtectionType](/cells/de/python-net/aspose.cells/protectiontype) | Schutzart.|
###  Bemerkungen

Diese Methode schützt das Arbeitsblatt ohne Passwort. Es kann protect Arbeitsblatt in allen Versionen der Excel-Datei.

##  protect(type, password, old_password) {#ProtectionType-str-str}

Schützt Arbeitsblatt.



```python
def protect(self, type, password, old_password):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| type | [ProtectionType](/cells/de/python-net/aspose.cells/protectiontype) | Schutzart.|
| password | str | Passwort.|
| old_password | str | Wenn das Arbeitsblatt bereits passwortgeschützt ist, geben Sie bitte das alte Passwort ein.<br/> Andernfalls können Sie für diesen Parameter einen Nullwert oder eine leere Zeichenfolge festlegen.|
###  Bemerkungen

Diese Methode kann protect Arbeitsblatt in allen Versionen der Excel-Datei.
###  Beispiel


```python
from aspose.cells import ProtectionType, Workbook

# Instantiating a Workbook object
excel = Workbook("template.xlsx")
# Accessing the first worksheet in the Excel file
worksheet = excel.worksheets[0]
# Protecting the worksheet with a password
worksheet.protect(ProtectionType.ALL, "aspose", None)
# Saving the modified Excel file in default (that is Excel 20003) format
excel.save("output.xls")

```



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Worksheet](/cells/de/python-net/aspose.cells/worksheet)

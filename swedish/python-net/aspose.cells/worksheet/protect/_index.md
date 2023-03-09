---
title: protect metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 180
url: /sv/python-net/aspose.cells/worksheet/protect/
is_root: false
---
##  protect(type) {#ProtectionType}
Skyddar kalkylblad.



```python
def protect(self, type):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| type | [ProtectionType](/cells/sv/python-net/aspose.cells/protectiontype) | Skyddstyp.|
###  Anmärkningar

Denna metod skyddar kalkylblad utan lösenord.

##  protect(type, password, old_password) {#ProtectionType-str-str}

Skyddar kalkylblad.



```python
def protect(self, type, password, old_password):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| type | [ProtectionType](/cells/sv/python-net/aspose.cells/protectiontype) | Skyddstyp.|
| password | str | Lösenord.|
| old_password | str | Om kalkylbladet redan är skyddat av ett lösenord, vänligen ange det gamla lösenordet.<br/> Annars kan du ställa in ett nollvärde eller tom sträng för denna parameter.|
###  Anmärkningar

Denna metod kan protect kalkylblad i alla versioner av Excel-fil.
###  Exempel


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



###  Se även
* modul [aspose.cells](../../)
* klass [Worksheet](/cells/sv/python-net/aspose.cells/worksheet)

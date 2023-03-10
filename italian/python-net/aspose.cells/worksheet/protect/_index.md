---
title: metodo protect
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 180
url: /it/python-net/aspose.cells/worksheet/protect/
is_root: false
---
##  protect(type) {#ProtectionType}
Protegge il foglio di lavoro.



```python
def protect(self, type):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| type | [ProtectionType](/cells/it/python-net/aspose.cells/protectiontype) | Tipo di protezione.|
###  Osservazioni

Questo metodo protegge il foglio di lavoro senza password. Può protect foglio di lavoro in tutte le versioni del file Excel.

##  protect(type, password, old_password) {#ProtectionType-str-str}

Protegge il foglio di lavoro.



```python
def protect(self, type, password, old_password):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| type | [ProtectionType](/cells/it/python-net/aspose.cells/protectiontype) | Tipo di protezione.|
| password | str | Parola d'ordine.|
| old_password | str | Se il foglio di lavoro è già protetto da una password, fornire la vecchia password.<br/> In caso contrario, è possibile impostare un valore nullo o una stringa vuota su questo parametro.|
###  Osservazioni

Questo metodo può protect foglio di lavoro in tutte le versioni del file Excel.
###  Esempio


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



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Worksheet](/cells/it/python-net/aspose.cells/worksheet)

---
title: protect method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 180
url: /python-net/aspose.cells/worksheet/protect/
is_root: false
---

## protect(type) {#ProtectionType}

Protects worksheet.



```python
def protect(self, type):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| type | [ProtectionType](/cells/python-net/aspose.cells/protectiontype) | Protection type. |
### Remarks

This method protects worksheet without password. It can protect worksheet in all versions of Excel file.

## protect(type, password, old_password) {#ProtectionType-str-str}

Protects worksheet.



```python
def protect(self, type, password, old_password):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| type | [ProtectionType](/cells/python-net/aspose.cells/protectiontype) | Protection type. |
| password | str | Password. |
| old_password | str | If the worksheet is already protected by a password, please supply the old password.<br/>Otherwise, you can set a null value or blank string to this parameter. |
### Remarks

This method can protect worksheet in all versions of Excel file.
### Example 


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



### See Also
* module [aspose.cells](../../)
* class [Worksheet](/cells/python-net/aspose.cells/worksheet)

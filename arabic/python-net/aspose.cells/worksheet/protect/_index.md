---
title: طريقة protect
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 180
url: /ar/python-net/aspose.cells/worksheet/protect/
is_root: false
---
##  protect(type) {#ProtectionType}
يحمي ورقة العمل.



```python
def protect(self, type):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| type | [ProtectionType](/cells/ar/python-net/aspose.cells/protectiontype) | نوع الحماية.|
###  ملاحظات

هذه الطريقة تحمي ورقة العمل بدون كلمة مرور.

##  protect(type, password, old_password) {#ProtectionType-str-str}

يحمي ورقة العمل.



```python
def protect(self, type, password, old_password):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| type | [ProtectionType](/cells/ar/python-net/aspose.cells/protectiontype) | نوع الحماية.|
| password | str | كلمة المرور.|
| old_password | str | إذا كانت ورقة العمل محمية بالفعل بكلمة مرور ، فيرجى توفير كلمة المرور القديمة.<br/> خلاف ذلك ، يمكنك تعيين قيمة فارغة أو سلسلة فارغة لهذه المعلمة.|
###  ملاحظات

يمكن لهذه الطريقة أن protect ورقة عمل في كافة إصدارات ملف Excel.
###  أمثلة


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



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Worksheet](/cells/ar/python-net/aspose.cells/worksheet)

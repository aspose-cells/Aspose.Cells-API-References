---
title: protect方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 180
url: /zh/python-net/aspose.cells/worksheet/protect/
is_root: false
---
##  protect(type) {#ProtectionType}
保护工作表。



```python
def protect(self, type):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| type | [ProtectionType](/cells/zh/python-net/aspose.cells/protectiontype) |保护类型。|
### 评论

此方法无需密码即可保护工作表。它可以在所有版本的 Excel 文件中生成 protect 工作表。

##  protect(type, password, old_password) {#ProtectionType-str-str}

保护工作表。



```python
def protect(self, type, password, old_password):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| type | [ProtectionType](/cells/zh/python-net/aspose.cells/protectiontype) |保护类型。|
| password | str |密码。|
| old_password | str |如果工作表已受密码保护，请提供旧密码。<br/>否则，您可以为此参数设置空值或空白字符串。|
### 评论

protect 这个方法可以在所有版本的Excel文件中使用工作表。
### 例子


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



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Worksheet](/cells/zh/python-net/aspose.cells/worksheet)

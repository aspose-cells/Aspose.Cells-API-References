---
title: check_excel_restriction 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 90
url: /zh/python-net/aspose.cells/htmlloadoptions/check_excel_restriction/
is_root: false
---
## check_excel_restriction 属性

用户修改单元格相关对象时是否检查excel文件的限制。
例如，excel 不允许输入超过 32K 的字符串值。
当您输入一个大于 32K 的值时，例如 Cell.PutValue(string)，如果此属性为真，您将得到一个异常。
如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便稍后
您可以输出其他文件格式的完整字符串值，例如 CSV。
但是，如果您设置了这种对 excel 文件格式无效的值，
您以后不应将工作簿另存为 excel 文件格式。否则生成的excel文件可能会出现意外错误。
### 定义：
```python
@property
def check_excel_restriction(self):
    ...
@check_excel_restriction.setter
def check_excel_restriction(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [HtmlLoadOptions](/cells/zh/python-net/aspose.cells/htmlloadoptions)

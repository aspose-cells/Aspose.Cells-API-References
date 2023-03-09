---
title: FormatConditionType枚举
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 2100
url: /zh/python-net/aspose.cells/formatconditiontype/
is_root: false
---
## FormatConditionType枚举
条件格式规则类型。



FormatConditionType 类型公开了以下成员：

### 字段
|场地|描述|
| :- | :- |
| CELL_VALUE |此条件格式规则比较单元格值<br/>到公式计算结果，使用运算符。|
| EXPRESSION |此条件格式规则包含一个公式<br/>求值。当公式结果为真时，单元格为<br/>突出显示。|
| COLOR_SCALE |此条件格式规则创建一个分级<br/>细胞上的色标。|
| DATA_BAR |此条件格式规则显示分级<br/>单元格区域中的数据栏。|
| ICON_SET |此条件格式规则将图标应用于单元格<br/>根据他们的价值观。|
| TOP10 |此条件格式规则突出显示其单元格<br/>值落在前 N 个或后 N 个括号中，如<br/>指定的。|
| UNIQUE_VALUES |此条件格式规则突出显示唯一<br/>范围内的值。|
| DUPLICATE_VALUES |此条件格式规则突出显示重复<br/>值。|
| CONTAINS_TEXT |此条件格式规则突出显示单元格<br/>包含给定文本。等同于使用 SEARCH()<br/>sheet函数判断单元格是否包含<br/>文本。|
| NOT_CONTAINS_TEXT |此条件格式规则突出显示单元格<br/>不包含给定的文本。<br/>sheet函数判断单元格是否包含<br/>文字与否。|
| BEGINS_WITH |此条件格式规则突出显示<br/>以给定文本开头的范围。<br/>使用 LEFT() 工作表函数并比较值。|
| ENDS_WITH |此条件格式规则突出显示单元格结尾<br/>给定的文本。等同于使用 RIGHT() 工作表<br/>函数和比较值。|
| CONTAINS_BLANKS |此条件格式规则突出显示单元格<br/>完全空白。等同于使用 LEN(TRIM())。<br/>这意味着如果单元格只包含字符<br/>TRIM() 将删除，然后它被认为是空白的。<br/>空单元格也被视为空白。|
| NOT_CONTAINS_BLANKS |此条件格式规则突出显示单元格<br/>不为空。等同于使用 LEN(TRIM())。<br/>意味着如果单元格只包含字符<br/>TRIM() 将删除，然后它被视为空白。<br/>空单元格也被视为空白。|
| CONTAINS_ERRORS |此条件格式规则突出显示单元格<br/>公式错误。相当于使用 ISERROR() 表<br/>函数判断是否有公式错误。|
| NOT_CONTAINS_ERRORS |此条件格式规则突出显示单元格<br/>没有公式错误。等同于使用 ISERROR()<br/> sheet函数判断是否有公式错误。|
| TIME_PERIOD |此条件格式规则突出显示单元格<br/>包含指定时间段内的日期。<br/>评估单元格的基础值，因此<br/>单元格不需要格式化为日期<br/>评估。例如，一个单元格包含<br/>值 38913 应应用条件格式，如果<br/>该规则要求值为 7/14/2006。|
| ABOVE_AVERAGE |此条件格式规则突出显示单元格<br/>高于或低于所有值的平均值<br/>范围。|



### 也可以看看
* 模块 [aspose.cells](..)

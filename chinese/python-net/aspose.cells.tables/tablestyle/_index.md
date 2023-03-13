---
title: TableStyle类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 50
url: /zh/python-net/aspose.cells.tables/tablestyle/
is_root: false
---
## TableStyle类
表示表格样式。



TableStyle 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [name](/cells/zh/python-net/aspose.cells.tables/tablestyle/name) |获取表格样式的名称。|
| [table_style_elements](/cells/zh/python-net/aspose.cells.tables/tablestyle/table_style_elements) |获取表格样式的所有元素。|



### 例子

```python
from aspose.cells import BackgroundType, CellsHelper, Workbook
from aspose.cells.tables import TableStyleElementType
from aspose.pydrawing import Color

workbook = Workbook()
firstColumnStyle = workbook.create_style()
firstColumnStyle.pattern = BackgroundType.SOLID
firstColumnStyle.background_color = Color.red
lastColumnStyle = workbook.create_style()
lastColumnStyle.font.is_bold = True
lastColumnStyle.pattern = BackgroundType.SOLID
lastColumnStyle.background_color = Color.red
tableStyleName = "Custom1"
tableStyles = workbook.worksheets.table_styles
index1 = tableStyles.add_table_style(tableStyleName)
tableStyle = tableStyles[index1]
elements = tableStyle.table_style_elements
index1 = elements.add(TableStyleElementType.FIRST_COLUMN)
element = elements[index1]
element.set_element_style(firstColumnStyle)
index1 = elements.add(TableStyleElementType.LAST_COLUMN)
element = elements[index1]
element.set_element_style(lastColumnStyle)
cells = workbook.worksheets[0].cells
for i in range(5):
    cells.get(0, i).put_value(CellsHelper.column_index_to_name(i))
for row in range(1, 10):
    for column in range(5):
        cells.get(row, column).put_value(row * column)
tables = workbook.worksheets[0].list_objects
index = tables.add(0, 0, 9, 4, True)
table = tables[0]
table.show_table_style_first_column = True
table.show_table_style_last_column = True
table.table_style_name = tableStyleName
workbook.save(r"Book1.xlsx")

```

### 也可以看看
* 模块 [aspose.cells.tables](..)

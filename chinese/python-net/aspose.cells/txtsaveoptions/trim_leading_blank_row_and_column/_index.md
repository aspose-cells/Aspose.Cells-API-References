---
title: trim_leading_blank_row_and_column 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 220
url: /zh/python-net/aspose.cells/txtsaveoptions/trim_leading_blank_row_and_column/
is_root: false
---
## trim_leading_blank_row_and_column 属性

指示是否应像 ms excel 那样修剪前导空白行和列。
默认为真。

### 评论

与ms excel中的规则相同，如果行/列具有自定义样式，则不会被视为空白，
即使它不包含单元格数据。
使用 LightCells 模式保存时，此选项无效。
用户应通过执行 [TxtSaveOptions.light_cells_data_provider](/cells/zh/python-net/aspose.cells/txtsaveoptions#light_cells_data_provider) 来控制输出范围
或指定 [TxtSaveOptions.export_area](/cells/zh/python-net/aspose.cells/txtsaveoptions#export_area)
### 定义：
```python
@property
def trim_leading_blank_row_and_column(self):
    ...
@trim_leading_blank_row_and_column.setter
def trim_leading_blank_row_and_column(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [TxtSaveOptions](/cells/zh/python-net/aspose.cells/txtsaveoptions)

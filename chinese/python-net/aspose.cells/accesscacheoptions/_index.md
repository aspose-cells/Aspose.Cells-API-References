---
title: AccessCacheOptions枚举
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 1740
url: /zh/python-net/aspose.cells/accesscacheoptions/
is_root: false
---
## AccessCacheOptions枚举
用于数据访问的缓存选项。可以与 | 运算符组合在一起使用多个选项。



AccessCacheOptions 类型公开了以下成员：

### 字段
|场地|描述|
| :- | :- |
| NONE |没有任何数据访问的缓存。|
| ALL |对工作簿中的各种数据访问应用所有可能的优化。<br/>在优化访问期间不应更改所有设置和数据。|
| POSITION_AND_SIZE |应用可能的优化来获取对象（例如形状）的位置和大小。<br/>在优化访问期间不应更改行高和列宽设置。|
| CELLS_DATA |应用可能的优化来获取单元格的值。<br/>Cells 数据（Cell 的数据和设置，行）不应在期间更改<br/>优化访问，也不应创建新的 Cell/Row 对象（例如<br/>通过 [[indexer]](/cells/python-net/aspose.cells/cells/__getitem__/)）。|
| CELL_DISPLAY |应用可能的优化以获得与显示相关的结果<br/>细胞（[Cell.display_string_value](/cells/zh/python-net/aspose.cells/cell#display_string_value)、[Cell.get_style()](/cells/zh/python-net/aspose.cells/cell/get_style)、[Cell.get_display_style()](/cells/zh/python-net/aspose.cells/cell/get_display_style) 等）。<br/>Cells 数据和样式相关的对象（Cell/Row/Column样式，列宽等）不应该改变<br/>在优化访问期间。|
| GET_FORMULA |应用可能的优化来获取公式。<br/>所有可能影响公式表达式的数据和设置（工作表的名称，名称的文本，<br/>表的列等）在优化访问期间不应更改。|
| SET_FORMULA |对设置公式应用可能的优化。<br/>所有可能影响公式表达式的数据和设置（工作表的名称，名称的文本，<br/>表的列等）在优化访问期间不应更改。|
| CALCULATE_FORMULA |对计算公式应用可能的优化。<br/>Cells 在优化访问期间不应更改数据，无新对象（Cell、Row 等）<br/>应该创建（例如 [[indexer]](/cells/python-net/aspose.cells/cells/__getitem__/)）。|
| CONDITIONAL_FORMATTING |应用可能的优化以获取条件格式的格式结果。<br/>所有可能影响条件格式结果的数据和设置（设置<br/>条件格式、相关单元格值等）在优化访问期间不应更改。|
| VALIDATION |应用可能的优化以获得验证结果。<br/>所有可能影响验证结果的数据和设置（settings of the validation,<br/>依赖的单元格值等）在优化访问期间不应更改。|



### 评论

对于某些特征，访问大型数据集需要大量重复和复杂的操作
例如搜索，计算，...等等，这些操作会花费很多额外的时间。
对于常见的情况，所有依赖的数据在访问过程中都保持不变，因此可以构建一些缓存用于
提高访问性能。
为此，我们提供了这个 API 以便用户可以指定需要哪种数据访问
通过可能的缓存机制进行优化。


请注意，对于不同的选项，不同的数据集可能需要“只读”。
而访问数据的性能取决于很多方面，缓存机制的使用
不保证性能会得到改善。
例如要访问的数据集很小，使用缓存可能会导致更多时间，因为
缓存本身也需要一定的额外时间。

### 也可以看看
* 模块 [aspose.cells](..)

---
title: LightCellsDataProvider类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 1000
url: /zh/python-net/aspose.cells/lightcellsdataprovider/
is_root: false
---
## LightCellsDataProvider类
表示用于在轻量级模式下保存大型电子表格文件的数据提供程序。



LightCellsDataProvider 类型公开了以下成员：

### 方法
|方法|描述|
| :- | :- |
| [start_sheet(sheet_index)](/cells/zh/python-net/aspose.cells/lightcellsdataprovider/start_sheet/#int) |开始保存工作表。|
| [next_row()](/cells/zh/python-net/aspose.cells/lightcellsdataprovider/next_row/#) |获取要保存的下一行。|
| [start_row(row)](/cells/zh/python-net/aspose.cells/lightcellsdataprovider/start_row/#Row) |开始保存一行数据。|
| [next_cell()](/cells/zh/python-net/aspose.cells/lightcellsdataprovider/next_cell/#) |获取下一个要保存的单元格。|
| [start_cell(cell)](/cells/zh/python-net/aspose.cells/lightcellsdataprovider/start_cell/#Cell) |开始保存一个单元格的数据。|
| [is_gather_string()](/cells/zh/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/#) |检查单元格的当前字符串值是否需要收集到全局池中。|



### 评论

用这种方式保存工作簿时，保存工作簿中的每张工作表时都会勾选[LightCellsDataProvider.start_sheet(sheet_index)](/cells/zh/python-net/aspose.cells/lightcellsdataprovider/start_sheet)。
对于一张工作表，如果 [LightCellsDataProvider.start_sheet(sheet_index)](/cells/zh/python-net/aspose.cells/lightcellsdataprovider/start_sheet) 为真，则将保存此工作表的行/单元格的所有数据和属性
将由该接口的实现提供。首先，将调用 [LightCellsDataProvider.next_row()](/cells/zh/python-net/aspose.cells/lightcellsdataprovider/next_row) 以获取要保存的下一行索引。
如果返回有效的行索引（行索引必须按升序排列才能保存行），
然后将提供一个表示该行的 Row 对象以供实现，以通过 [LightCellsDataProvider.start_row(row)](/cells/zh/python-net/aspose.cells/lightcellsdataprovider/start_row) 设置其属性。
对于一行，首先检查 [LightCellsDataProvider.next_cell()](/cells/zh/python-net/aspose.cells/lightcellsdataprovider/next_cell) 如果返回有效的列索引（列索引必须按升序排列才能保存一行的所有单元格），
然后将提供表示此单元格的 Cell 对象以供实现，以通过 [LightCellsDataProvider.start_cell(cell)](/cells/zh/python-net/aspose.cells/lightcellsdataprovider/start_cell) 设置其数据和属性。
设置好该单元格的数据后，该单元格将直接保存到生成的电子表格文件中，并检查处理下一个单元格。

### 也可以看看
* 模块 [aspose.cells](..)

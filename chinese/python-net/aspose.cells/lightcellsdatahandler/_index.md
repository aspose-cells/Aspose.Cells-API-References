---
title: LightCellsDataHandler类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 990
url: /zh/python-net/aspose.cells/lightcellsdatahandler/
is_root: false
---
##  LightCellsDataHandler类
表示用于在轻量级模式下读取大型电子表格文件的单元格数据处理程序。



LightCellsDataHandler 类型公开了以下成员：

### 方法
|方法|描述|
| :- | :- |
| [start_sheet(sheet)](/cells/zh/python-net/aspose.cells/lightcellsdatahandler/start_sheet/#Worksheet) |开始处理工作表。|
| [start_row(row_index)](/cells/zh/python-net/aspose.cells/lightcellsdatahandler/start_row/#int) |准备处理一行。|
| [process_row(row)](/cells/zh/python-net/aspose.cells/lightcellsdatahandler/process_row/#Row) |开始处理一行。|
| [start_cell(column_index)](/cells/zh/python-net/aspose.cells/lightcellsdatahandler/start_cell/#int) |准备处理一个单元格。|
| [process_cell(cell)](/cells/zh/python-net/aspose.cells/lightcellsdatahandler/process_cell/#Cell) |开始处理一个细胞。|



### 评论

使用该模式读取工作簿时，读取工作簿中的每张工作表时都会检查[LightCellsDataHandler.start_sheet(sheet)](/cells/zh/python-net/aspose.cells/lightcellsdatahandler/start_sheet)。
对于一张工作表，如果 [LightCellsDataHandler.start_sheet(sheet)](/cells/zh/python-net/aspose.cells/lightcellsdatahandler/start_sheet) 为真，则将检查该工作表的行/单元格的所有数据和属性
并由该接口的实现处理。对于每一行，都会调用 [LightCellsDataHandler.start_row(row_index)](/cells/zh/python-net/aspose.cells/lightcellsdatahandler/start_row) 来检查是否需要处理。
如果需要处理一行，则首先读取该行的属性，用户可以通过 [LightCellsDataHandler.process_row(row)](/cells/zh/python-net/aspose.cells/lightcellsdatahandler/process_row) 访问其属性。
如果行的单元格也需要处理，那么 [LightCellsDataHandler.process_row(row)](/cells/zh/python-net/aspose.cells/lightcellsdatahandler/process_row) 应该返回 true 然后 [LightCellsDataHandler.start_cell(column_index)](/cells/zh/python-net/aspose.cells/lightcellsdatahandler/start_cell) 将是
要求此行中的每个现有单元格检查是否需要处理一个单元格。如果需要处理一个单元格，
然后调用 [LightCellsDataHandler.process_cell(cell)](/cells/zh/python-net/aspose.cells/lightcellsdatahandler/process_cell) 来处理这个接口的实现。

### 也可以看看
* 模块 [aspose.cells](..)

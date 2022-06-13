---
title: GridDesktop
second_title: Aspose.Cells for .NET API 参考
description: Aspose GridDesktop 类 表示创建 GridDesktop 控件的根对象要使用此控件只需将其从工具箱拖到窗体或用户控件
type: docs
weight: 840
url: /zh/net/aspose.cells.griddesktop/griddesktop/
---
## GridDesktop class

Aspose GridDesktop 类 表示创建 GridDesktop 控件的根对象。要使用此控件，只需将其从工具箱拖到窗体或用户控件。

```csharp
public class GridDesktop : UserControl
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [GridDesktop](griddesktop)() | Aspose GridDesktop 类 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells.griddesktop/griddesktop/activesheetindex) { get; set; } | 获取或设置选定的工作表索引。 |
| [ActiveSheetNameFont](../../aspose.cells.griddesktop/griddesktop/activesheetnamefont) { get; set; } | 获取或设置表单栏的活动表单显示字体。 |
| [AlwasysRecalculateAllFormulas](../../aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas) { get; set; } | 获取或设置一个值，指示我们是否需要运行所有公式，如运行所有公式时， 更新一个单元格值时，以及它影响别人，别人影响别人，越来越多， 导致整个细胞需要重新计算，就像蝴蝶效应一样，它需要大量的堆栈操作， 它会得到非常低的性能， 就像在 CELLSNET-41921 中一样，这个问题包含可以显示这种情况的文件 我们最好只运行所有公式， ，当运行所有公式时，我们可能会进行一些优化。 |
| [BorderStyle](../../aspose.cells.griddesktop/griddesktop/borderstyle) { get; set; } | 表示控件的边框样式。 |
| [ColumnHeaderVisible](../../aspose.cells.griddesktop/griddesktop/columnheadervisible) { get; set; } | 获取或设置一个指示列标题是否可见的值。 |
| [CommentDisplayingFont](../../aspose.cells.griddesktop/griddesktop/commentdisplayingfont) { get; set; } | 获取或设置评论文本的默认显示字体。 |
| [ContextMenuManager](../../aspose.cells.griddesktop/griddesktop/contextmenumanager) { get; } | 获取 ContextMenuManager 实例。 |
| [DefaultCellFont](../../aspose.cells.griddesktop/griddesktop/defaultcellfont) { get; set; } | 获取或设置单元格的默认字体 |
| [DefaultCellFontColor](../../aspose.cells.griddesktop/griddesktop/defaultcellfontcolor) { get; set; } | 获取或设置单元格的默认字体颜色。 |
| [EnableClipboardCopyPaste](../../aspose.cells.griddesktop/griddesktop/enableclipboardcopypaste) { get; set; } | 表示是否根据剪贴板进行复制/粘贴，以便用MS-EXCEL进行复制/粘贴。 仅复制/粘贴单元格值，不复制单元格的任何其他设置，如格式、边框样式等 默认值为 false。 |
| [EnableCopyWithExtension](../../aspose.cells.griddesktop/griddesktop/enablecopywithextension) { get; set; } | 获取或设置一个值，该值指示复制操作是否将扩展行数或列数。 |
| [EnableCopyWithLockedOption](../../aspose.cells.griddesktop/griddesktop/enablecopywithlockedoption) { get; set; } | 获取或设置一个值，该值指示复制操作是否将复制单元格的样式的 CellLocked 属性值。 |
| [EnableUndo](../../aspose.cells.griddesktop/griddesktop/enableundo) { get; set; } | 获取或设置一个值，该值指示是否启用撤消功能。默认值为假。 |
| [GridMemorySetting](../../aspose.cells.griddesktop/griddesktop/gridmemorysetting) { get; set; } | 获取或设置内存选项。 |
| [IsHorizontalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/ishorizontalscrollbarvisible) { get; set; } | 设置水平滚动条的可见状态。 |
| [IsVerticalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/isverticalscrollbarvisible) { get; set; } | 设置垂直滚动条的可见雕像。 |
| [Names](../../aspose.cells.griddesktop/griddesktop/names) { get; } | 获取电子表格中所有 Name 对象的集合。 |
| [PageRows](../../aspose.cells.griddesktop/griddesktop/pagerows) { get; set; } | 设置或获取分页的行大小。支持的最大 PageRows 为 100000，支持的最大页码为 5000。 |
| [PasteType](../../aspose.cells.griddesktop/griddesktop/pastetype) { get; set; } | 表示粘贴动作时的粘贴类型，仅在 EnableClipboardCopyPaste 为 false 时可用。 |
| [R1C1](../../aspose.cells.griddesktop/griddesktop/r1c1) { get; set; } | 获取或设置一个值，该值指示控件是否使用 R1C1 引用样式。 |
| [RecalculateFormulas](../../aspose.cells.griddesktop/griddesktop/recalculateformulas) { get; set; } | 获取或设置一个值，该值指示当单元格的值发生变化时是否重新计算 所有单元格的公式。 默认值为真。 |
| [RowHeaderVisible](../../aspose.cells.griddesktop/griddesktop/rowheadervisible) { get; set; } | 获取或设置指示行标题是否可见的值。 |
| [SheetNameFont](../../aspose.cells.griddesktop/griddesktop/sheetnamefont) { get; set; } | 获取或设置表单栏的默认显示字体。 |
| [SheetsBarVisible](../../aspose.cells.griddesktop/griddesktop/sheetsbarvisible) { get; set; } | 获取或设置一个指示工作表栏是否可见的值。 |
| [SheetTabWidth](../../aspose.cells.griddesktop/griddesktop/sheettabwidth) { get; set; } | 设置/获取工作表选项卡的宽度。 |
| [ShowContextMenu](../../aspose.cells.griddesktop/griddesktop/showcontextmenu) { get; set; } | 获取或设置一个值，该值指示控件是否可以显示上下文菜单。 |
| [ShowStatus](../../aspose.cells.griddesktop/griddesktop/showstatus) { get; set; } | 获取或设置是否显示计算状态的值 默认值为true。 |
| [UndoManager](../../aspose.cells.griddesktop/griddesktop/undomanager) { get; } | 获取 UndoManager 实例。 |
| [Worksheets](../../aspose.cells.griddesktop/griddesktop/worksheets) { get; } | 获取工作表。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Clear](../../aspose.cells.griddesktop/griddesktop/clear)() | 清除 GridDesktop 控件。 |
| [Copy](../../aspose.cells.griddesktop/griddesktop/copy)() | 将焦点单元格内容复制到剪贴板。 |
| [Cut](../../aspose.cells.griddesktop/griddesktop/cut)() | 将焦点单元格内容剪切到剪贴板。 |
| [DoSplit](../../aspose.cells.griddesktop/griddesktop/dosplit)() | 设置拆分视图。 |
| [EndFormatPainter](../../aspose.cells.griddesktop/griddesktop/endformatpainter)() | 通知 GridDesktop 结束 FormatPainter。 |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile)(Stream) | 导出到excel文件流，包括磁盘IO流或者内存流。 |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile_2)(string) | 导出到 Excel 文件。 |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile_1)(Stream, FileFormatType) | 导出到excel文件流，包括磁盘IO流或者内存流。 |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile_3)(string, FileFormatType) | 导出到 Excel 文件。 |
| [GetActiveWorksheet](../../aspose.cells.griddesktop/griddesktop/getactiveworksheet)() | 获取当前活动工作表。 |
| [getHScrollBar](../../aspose.cells.griddesktop/griddesktop/gethscrollbar)() | 返回水平滚动条 |
| [getVScrollBar](../../aspose.cells.griddesktop/griddesktop/getvscrollbar)() | 返回垂直滚动条 |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile)(Stream) | 从 excel 文件流导入，包括磁盘文件流或内存流。 |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_3)(string) | 从 excel 文件导入。 |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_1)(Stream, bool) | 从 excel 文件流导入，包括磁盘文件流或内存流。 |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_4)(string, bool) | 从 excel 文件导入。 |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_5)(string, int) | 从 Excel 文件导入工作表。 |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_2)(Stream, string, string, bool, bool) | 从 excel 文件导入。 |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_6)(string, string, string, bool, bool) | 从 excel 文件导入。 |
| [OpenFindReplaceDialog](../../aspose.cells.griddesktop/griddesktop/openfindreplacedialog)(bool) | 打开 FindReplace 对话框以查找或替换单元格。 |
| [Paste](../../aspose.cells.griddesktop/griddesktop/paste)() | 将剪贴板内容粘贴到焦点单元格。 |
| [RefreshControl](../../aspose.cells.griddesktop/griddesktop/refreshcontrol)() | 刷新 GridDesktop 控件。 |
| [RunAllFormulas](../../aspose.cells.griddesktop/griddesktop/runallformulas)() | 运行所有单元格的公式。 |
| [SetAllScrollBarsVisible](../../aspose.cells.griddesktop/griddesktop/setallscrollbarsvisible)() | 设置所有滚动条可见。 |
| [ShowStyleDialog](../../aspose.cells.griddesktop/griddesktop/showstyledialog)() | 打开样式对话框，设置单元格样式、字体、颜色等 |
| [StartFormatPainter](../../aspose.cells.griddesktop/griddesktop/startformatpainter)(bool) | 通知 GridDesktop 启动 FormatPainter。 |
| [UnDoSplit](../../aspose.cells.griddesktop/griddesktop/undosplit)() | 取消设置拆分视图。 |
| static [GetVersion](../../aspose.cells.griddesktop/griddesktop/getversion)() | 获取发布版本。 |

## 字段

| 姓名 | 描述 |
| --- | --- |
| [LoadDataFilter](../../aspose.cells.griddesktop/griddesktop/loaddatafilter) | 从模板加载工作簿时过滤数据的选项。 |
| [ShowImportMessage](../../aspose.cells.griddesktop/griddesktop/showimportmessage) | 导入文件失败时是否显示消息框，默认值为真 |

## 活动

| 姓名 | 描述 |
| --- | --- |
| event [AfterDeleteColumns](../../aspose.cells.griddesktop/griddesktop/afterdeletecolumns) | 在删除列后发生。 |
| event [AfterDeleteRows](../../aspose.cells.griddesktop/griddesktop/afterdeleterows) | 删除行后发生。 |
| event [AfterInsertColumns](../../aspose.cells.griddesktop/griddesktop/afterinsertcolumns) | 在插入新列后发生。 |
| event [AfterInsertRows](../../aspose.cells.griddesktop/griddesktop/afterinsertrows) | 在插入新行后发生。 |
| event [BeforeCalculate](../../aspose.cells.griddesktop/griddesktop/beforecalculate) | 在工作簿中的计算公式之前发生。 |
| event [BeforeLoadFile](../../aspose.cells.griddesktop/griddesktop/beforeloadfile) | 在从文件加载工作簿之前发生。 |
| event [CellButtonClick](../../aspose.cells.griddesktop/griddesktop/cellbuttonclick) | 在单击单元格按钮时发生。 |
| event [CellCheckedChanged](../../aspose.cells.griddesktop/griddesktop/cellcheckedchanged) | 在更改单元格复选框 Checked 属性时发生。 |
| event [CellClick](../../aspose.cells.griddesktop/griddesktop/cellclick) | 在单击网格单元时发生。 |
| event [CellComboBoxCopy](../../aspose.cells.griddesktop/griddesktop/cellcomboboxcopy) | 在复制网格单元格 ComboBox 时发生。 |
| event [CellDataChanged](../../aspose.cells.griddesktop/griddesktop/celldatachanged) | 在网格单元格数据属性更改时发生。 |
| event [CellDoubleClick](../../aspose.cells.griddesktop/griddesktop/celldoubleclick) | 双击网格单元格时发生。 |
| event [CellFormatChanged](../../aspose.cells.griddesktop/griddesktop/cellformatchanged) | 当通过单元格格式对话框更改单元格格式时发生。 |
| event [CellKeyPressed](../../aspose.cells.griddesktop/griddesktop/cellkeypressed) | 在单元格具有焦点时按下键时发生。 |
| event [CellSelectedIndexChanged](../../aspose.cells.griddesktop/griddesktop/cellselectedindexchanged) | 在单元格组合框 SelectedIndex 属性发生更改时发生。 |
| event [CellTextBoxChanging](../../aspose.cells.griddesktop/griddesktop/celltextboxchanging) | 在网格单元格中键入字符时发生。 |
| event [CellValidationFailed](../../aspose.cells.griddesktop/griddesktop/cellvalidationfailed) | 当网格单元验证失败时发生。 |
| event [ColumnHeaderClick](../../aspose.cells.griddesktop/griddesktop/columnheaderclick) | 在单击列标题时发生。 |
| event [ColumnHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/columnheaderdoubleclick) | 双击列标题时发生。 |
| event [CommentDataChanged](../../aspose.cells.griddesktop/griddesktop/commentdatachanged) | 在评论数据发生变化时发生。 |
| event [FailLoadFile](../../aspose.cells.griddesktop/griddesktop/failloadfile) |  |
| event [FinishCalculate](../../aspose.cells.griddesktop/griddesktop/finishcalculate) | 在工作簿中的计算公式之后发生。 |
| event [FinishLoadFile](../../aspose.cells.griddesktop/griddesktop/finishloadfile) | 在加载工作簿时发生。 |
| event [FocusedCellChanged](../../aspose.cells.griddesktop/griddesktop/focusedcellchanged) | 当焦点单元格改变时发生。 |
| event [RowColumnHiddenChanged](../../aspose.cells.griddesktop/griddesktop/rowcolumnhiddenchanged) | 当行/列隐藏状态改变时发生。 |
| event [RowFilteredEvent](../../aspose.cells.griddesktop/griddesktop/rowfilteredevent) | 在选择行过滤器项后发生。 |
| event [RowHeaderClick](../../aspose.cells.griddesktop/griddesktop/rowheaderclick) | 在单击行标题时发生。 |
| event [RowHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/rowheaderdoubleclick) | 双击行标题时发生。 |
| event [SelectedCellRangeChanged](../../aspose.cells.griddesktop/griddesktop/selectedcellrangechanged) | 在选定单元格范围更改时发生。 |
| event [SelectedSheetIndexChanged](../../aspose.cells.griddesktop/griddesktop/selectedsheetindexchanged) | 在 SelectedSheetIndex 属性更改时发生。 |
| event [ShapeClick](../../aspose.cells.griddesktop/griddesktop/shapeclick) | 单击形状时发生。 |

### 评论

有关 System.Windows.Forms.UserControl 的更多信息，请参阅 .NET SDK 文档。

### 例子

```csharp
[C#]
gridDesktop1.Worksheets[0].Cells[0, 0].Value = "2";
gridDesktop1.Worksheets[0].Cells[1, 0].Value = "3";
gridDesktop1.Worksheets[0].Cells[2, 1].Value = "=a1*a2";
gridDesktop1.RunAllFormulas();
gridDesktop1.Invalidate();

[Visual Basic]
gridDesktop1.Worksheets(0).Cells(0, 0).Value = "2"
gridDesktop1.Worksheets(0).Cells(1, 0).Value = "3"
gridDesktop1.Worksheets(0).Cells(2, 1).Value = "=a1*a2"
gridDesktop1.RunAllFormulas()
gridDesktop1.Invalidate()

```

### 也可以看看

* 命名空间 [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop)
* 部件 [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->

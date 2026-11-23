---
title: "类 WebWorksheet"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridWeb.Data.WebWorksheet 类。表示一个 Web 工作表"
type: docs
url: /zh/net/aspose.cells.gridweb.data/webworksheet/
---
## WebWorksheet class

表示一个 Web 工作表。

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet instead")]
public class WebWorksheet : Control, ISerializable
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [WebWorksheet](webworksheet/#constructor)() | WebWorksheet 的构造函数。 |
| [WebWorksheet](webworksheet/#constructor_1)(MainWeb, GridWorksheet) | WebWorksheet 的构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | 绑定列集合。 |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | 运行时实际绑定的数据源对象。当 DataSource 属性是 DataSet、DataTable 或 DataView 对象时，它是 DataView 对象。 |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | 在数据绑定模式下，BindStartRow 和 BindStartColumn 指示网格绑定到数据源的位置。 |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | 在数据绑定模式下，BindStartRow 和 BindStartColumn 指示网格绑定到数据源的位置。 |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } |  |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | 获取 [`WebCells`](../webcells/)。 |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } |  |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | 获取数据绑定模式下的绑定行数。 |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | 获取或设置来自多成员 DataSource 的 DataMember。通常它表示 DataSet 的 DataTable 对象。 |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | 获取或设置 DataSource。通常它是 DataSet 对象。 |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | 在数据绑定模式下，指示是否在工作表中创建绑定列标题。 |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | 获取 HyperlinkCollection 集合。 |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | 获取其在工作表集合中的索引。 |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | 获取或设置工作表是否受保护。当工作表受保护时，除 IsLocked 属性为 false 的单元格外，所有单元格均不可编辑。 |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | 获取或设置工作表的名称。 |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } |  |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | 获取工作表中的数据验证设置集合。 |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | 指示是否在控件的工作表标签中显示此工作表的名称。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn)(int) | 自动调整列宽。 |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | 自动调整列宽。此方法根据列中从 startRow 到 endRow 的单元格范围内容自动调整列宽。AutoFitColumn 是一个不精确的函数。 |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | 取消并删除新添加的绑定行。 |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | 提交新添加的绑定行并将其添加到数据源。 |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | 从另一个工作表对象复制。 |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | 为工作表设置数据源后，调用此方法自动生成绑定列。 |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | 创建一个新的绑定行并绑定到数据源。 |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | 在工作表中创建小计。 |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | 将工作表绑定到数据源。 |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | 删除绑定行。 |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | 在工作表的指定单元格处冻结窗格。 |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows)(int, int) | 对行进行分组。 |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows_1)(int, int, bool) | 对行进行分组。 |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | 使所有单元格可编辑。这是扩展属性。 |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | 使所有单元格只读。这是扩展属性，注意此属性不能保存在实际单元格中，如果想保持保护，请使用 setProtect。 |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | 使一段单元格可编辑。http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells 通过调用 SetAllCellsReadonly 方法将所有单元格设为只读。然后调用此方法指定要可编辑的单元格范围。 |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | 使一段单元格只读。http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells 首先通过调用 SetAllCellsEditable 方法将所有单元格设为可编辑。然后调用此方法指定要只读的单元格范围。 |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | 取消工作表中的窗格冻结。 |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | 取消行分组。 |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | 根据单元格的值更新绑定数据源记录的属性值。 |

### 备注

注意：此类已过时，请改用 GridWorksheet。该类将在自 2014 年 8 月起的 6 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp

 [C#]
 ...
 using System.Web.UI.WebControls;
 ...
 ...

 WebWorksheets Worksheets = GridWeb1.WebWorksheets;
	WebCells cells = Worksheets[0].Cells;

	//设置默认行高
	cells.StandardHeight = new Unit(16, UnitType.Point);
	//设置行高
	cells.SetRowHeight(2, new Unit(20, UnitType.Point));

	//设置默认列宽
	cells.StandardWidth = new Unit(50, UnitType.Point);
	//设置列宽
	cells.SetColumnWidth(3, new Unit(80, UnitType.Point));

	//合并单元格
	cells.Merge(5, 4, 2, 2);

	//导入数据
	DataSet1 ds1 = new DataSet1();

	for (int i =0; i<16; i++)
	{
		DataSet1.Table1Row row = ds1.Table1.NewTable1Row();
		row["c1"] = "hello1";
		row["c2"] = i;
		row["c3"] = "data";
		ds1.Table1.AddTable1Row(row);
	}

	GridWeb1.WebWorksheets.ImportDataView(ds1.Table1.DefaultView, null, null);

 //从 Excel 文件导入
 Worksheets.ImportExcelFile("c:\\file1.xls");

 [Visual Basic]
	Imports System.Web.UI.WebControls
	...
	...

	Dim Worksheets As WebWorksheets =  GridWeb1.WebWorksheets
	Dim cells As WebCells =  Worksheets(0).Cells

	'Sets default row height
	cells.StandardHeight = New Unit(16, UnitType.Point)
	'Sets row height
	cells.SetRowHeight(2,New Unit(20,UnitType.Point))

	'Sets default colum width
	cells.StandardWidth = New Unit(50, UnitType.Point)
	'Sets column width
	cells.SetColumnWidth(3,New Unit(80,UnitType.Point))

	'Merge cells
	cells.Merge(5, 4, 2, 2)

	'Import data
	Dim ds1 As DataSet1 =  New DataSet1()

	Dim i As Integer
	For  i = 0 To 15
		Dim row As DataSet1.Table1Row =  ds1.Table1.NewTable1Row()
		row("c1") = "hello1"
		row("c2") = i
		row("c3") = "data"
		ds1.Table1.AddTable1Row(row)
	Next

	GridWeb1.WebWorksheets.ImportDataView(ds1.Table1.DefaultView, Nothing, Nothing)

	'Import from excel file
	Worksheets.ImportExcelFile("c:\\file1.xls")
```

### 另请参见

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)



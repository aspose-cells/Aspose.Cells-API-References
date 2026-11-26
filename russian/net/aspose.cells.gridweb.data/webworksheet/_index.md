---
title: "Класс WebWorksheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.Data.WebWorksheet. Представляет веб-лист."
type: docs
url: /ru/net/aspose.cells.gridweb.data/webworksheet/
---
## WebWorksheet class

Представляет веб‑лист.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet instead")]
public class WebWorksheet : Control, ISerializable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WebWorksheet](webworksheet/#constructor)() | Конструктор WebWorksheet. |
| [WebWorksheet](webworksheet/#constructor_1)(MainWeb, GridWorksheet) | Конструктор WebWorksheet. |

## Свойства

| Имя | Описание |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | Привяжите коллекцию столбцов. |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | Фактический объект источника данных, привязываемый во время выполнения. Это объект DataView, когда свойство DataSource является объектом DataSet, DataTable или DataView. |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | В режиме привязки данных BindStartRow и BindStartColumn указывают позицию сетки для привязки к источнику данных. |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | В режиме привязки данных BindStartRow и BindStartColumn указывают позицию сетки для привязки к источнику данных. |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } |  |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | Получает [`WebCells`](../webcells/). |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } |  |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | Получает количество привязанных строк в режиме привязки данных. |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | Получает или задает DataMember из многокомпонентного DataSource. Обычно он представляет объект DataTable из DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | Получает или задает DataSource. Обычно это объект DataSet. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | В режиме привязки данных указывает, следует ли создавать подписи заголовков привязанных столбцов на листе. |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | Получает коллекцию HyperlinkCollection. |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | Получает индекс самого себя среди листов. |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | Получает или задает, защищён ли лист. Когда лист защищён, все ячейки нельзя редактировать, кроме ячейки, у которой свойство IsLocked равно false. |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | Получает или задает имя листа. |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } |  |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | Получает коллекцию настроек проверки данных в листе. |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | Указывает, отображается ли имя этого листа во вкладках листов управления. |

## Методы

| Имя | Описание |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn)(int) | Автоматически подгоняет ширину столбца. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Автоматически подгоняет ширину столбца. Этот метод подгоняет столбец по содержимому в диапазоне ячеек столбца от startRow до endRow. AutoFitColumn — неточная функция. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | Отменяет и удаляет только что добавленную привязанную строку. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | Подтверждает только что добавленную привязанную строку и добавляет её в datasource. |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | Копирует из другого объекта листа. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | После установки datasource для листа вызовите этот метод для автоматического создания привязанных столбцов. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | Создаёт новую привязанную строку и привязывает её к datasource. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Создаёт промежуточный итог на листе. |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | Привяжите лист к DataSource. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | Удаляет привязанную строку. |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | Замораживает области в указанной ячейке листа. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows)(int, int) | Группирует строки. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows_1)(int, int, bool) | Группирует строки. |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | Делает все ячейки редактируемыми. Это расширенный атрибут. |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | Делает все ячейки только для чтения. Это расширенный атрибут; обратите внимание, что этот атрибут не сохраняется в реальной ячейке, если нужно сохранить защиту, используйте setProtect. |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | Делает диапазон ячеек редактируемым. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Сделайте все ячейки только для чтения, вызвав метод SetAllCellsReadonly. Затем вызовите этот метод, чтобы указать диапазон ячеек, который будет редактируемым. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | Делает диапазон ячеек только для чтения. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Сначала сделайте все ячейки редактируемыми, вызвав метод SetAllCellsEditable. Затем вызовите этот метод, чтобы указать диапазон ячеек, который будет только для чтения. |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | Размораживает области в листе. |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | Разгруппирует строки. |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | Обновляет значение свойства записи источника данных привязки в соответствии со значением ячейки. |

### Примечания

ПРИМЕЧАНИЕ: Этот класс теперь устарел. пожалуйста, используйте GridWorksheet вместо него. Этот класс будет удалён через 6 месяцев после августа 2014 г. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp

 [C#]
 ...
 using System.Web.UI.WebControls;
 ...
 ...

 WebWorksheets Worksheets = GridWeb1.WebWorksheets;
	WebCells cells = Worksheets[0].Cells;

	//Устанавливает высоту строки по умолчанию
	cells.StandardHeight = new Unit(16, UnitType.Point);
	//Устанавливает высоту строки
	cells.SetRowHeight(2, new Unit(20, UnitType.Point));

	//Устанавливает ширину столбца по умолчанию
	cells.StandardWidth = new Unit(50, UnitType.Point);
	//Устанавливает ширину столбца
	cells.SetColumnWidth(3, new Unit(80, UnitType.Point));

	//Объединить ячейки
	cells.Merge(5, 4, 2, 2);

	//Импортировать данные
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

 //Импортировать из файла Excel
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

### См. также

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)



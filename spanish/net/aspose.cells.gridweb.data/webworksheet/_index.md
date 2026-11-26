---
title: "Clase WebWorksheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.GridWeb.Data.WebWorksheet class. Representa una hoja de cálculo web"
type: docs
url: /es/net/aspose.cells.gridweb.data/webworksheet/
---
## WebWorksheet class

Representa una hoja de cálculo web.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet instead")]
public class WebWorksheet : Control, ISerializable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [WebWorksheet](webworksheet/#constructor)() | el constructor de WebWorksheet. |
| [WebWorksheet](webworksheet/#constructor_1)(MainWeb, GridWorksheet) | el constructor de WebWorksheet. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | Vincule la colección de columnas. |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | El objeto de origen de datos realmente enlazado en tiempo de ejecución. Es un objeto DataView cuando la propiedad DataSource es un objeto DataSet, DataTable o DataView. |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar al origen de datos. |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar al origen de datos. |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } |  |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | Obtiene los [`WebCells`](../webcells/). |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } |  |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | Obtiene el número de filas vinculadas en modo de enlace de datos. |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | Obtiene o establece el DataMember del DataSource de múltiples miembros. Generalmente representa un objeto DataTable de un DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | Obtiene o establece el DataSource. Generalmente es un objeto DataSet. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | En modo de enlace de datos, indica si se deben crear los encabezados de columna vinculados en la hoja. |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | Obtiene la colección HyperlinkCollection. |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | Obtiene el índice de sí mismo dentro de las hojas de cálculo. |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | Obtiene o establece si la hoja de cálculo está protegida. Cuando una hoja de cálculo está protegida, todas las celdas no pueden editarse excepto la celda cuya propiedad IsLocked es false. |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | Obtiene o establece el nombre de la hoja. |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } |  |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | Obtiene la colección de configuraciones de validación de datos en la hoja de cálculo. |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | Indica si el nombre de esta hoja se muestra en las pestañas de hoja del control. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn)(int) | Ajusta automáticamente el ancho de la columna. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Ajusta automáticamente el ancho de la columna. Este método ajusta automáticamente una columna basándose en el contenido de un rango de celdas dentro de la columna desde startRow hasta endRow. AutoFitColumn es una función imprecisa. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | Cancela y elimina la fila vinculada recién añadida. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | Confirma la fila vinculada recién añadida y la agrega al datasource. |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | Copia de otro objeto de hoja de cálculo. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | Después de establecer un datasource para la hoja de cálculo, llame a este método para generar automáticamente las columnas vinculadas. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | Crea una nueva fila vinculada y la enlaza al datasource. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Crea un subtotal en la hoja. |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | Vincula la hoja al DataSource. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | Elimina una fila vinculada. |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | Congela paneles en la celda especificada de la hoja de cálculo. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows)(int, int) | Agrupa filas. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows_1)(int, int, bool) | Agrupa filas. |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | Hace que todas las celdas sean editables.este es un atributo extendido |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | Hace que todas las celdas sean de solo lectura.este es un atributo extendido, tenga en cuenta que este atributo no se conserva en la celda real, si desea mantener la protección, use setProtect |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | Hace que un rango de celdas sea editable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Haga que todas las celdas sean de solo lectura llamando al método SetAllCellsReadonly. luego llame a este método para especificar el rango de celdas que deben ser editables |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | Hace que un rango de celdas sea de solo lectura. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Primero haga que todas las celdas sean editables llamando al método SetAllCellsEditable. luego llame a este método para especificar el rango de celdas que deben ser de solo lectura |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | Descongela los paneles en la hoja de cálculo. |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | Desagrupa filas. |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | Actualiza el valor de la propiedad del registro de origen de datos de enlace según el valor de la celda. |

### Observaciones

NOTA: Esta clase está ahora obsoleta. Por favor use GridWorksheet en su lugar. Esta clase será eliminada después de 6 meses desde agosto de 2014. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp

 [C#]
 ...
 using System.Web.UI.WebControls;
 ...
 ...

 WebWorksheets Worksheets = GridWeb1.WebWorksheets;
	WebCells cells = Worksheets[0].Cells;

	//Establece la altura predeterminada de la fila
	cells.StandardHeight = new Unit(16, UnitType.Point);
	//Establece la altura de la fila
	cells.SetRowHeight(2, new Unit(20, UnitType.Point));

	//Establece el ancho predeterminado de la columna
	cells.StandardWidth = new Unit(50, UnitType.Point);
	//Establece el ancho de la columna
	cells.SetColumnWidth(3, new Unit(80, UnitType.Point));

	//Combinar celdas
	cells.Merge(5, 4, 2, 2);

	//Importar datos
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

 //Importar desde archivo de Excel
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

### Ver también

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)



---
title: "Klass WebWorksheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.WebWorksheet class. Representerar ett webb-arbetsblad"
type: docs
url: /sv/net/aspose.cells.gridweb.data/webworksheet/
---
## WebWorksheet class

Representerar ett webb‑arbetsblad.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet instead")]
public class WebWorksheet : Control, ISerializable
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [WebWorksheet](webworksheet/#constructor)() | konstruktorn för WebWorksheet. |
| [WebWorksheet](webworksheet/#constructor_1)(MainWeb, GridWorksheet) | konstruktorn för WebWorksheet. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | Bind kolumnsamling. |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | Det faktiska bindningsdatakällobjektet vid körning. Det är ett DataView-objekt när DataSource-egenskapen är ett DataSet-, DataTable- eller DataView-objekt. |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | I datakopplingsläge indikerar BindStartRow och BindStartColumn positionen för rutnätet som ska bindas till datakällan. |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | I datakopplingsläge indikerar BindStartRow och BindStartColumn positionen för rutnätet som ska bindas till datakällan. |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } |  |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | Hämtar [`WebCells`](../webcells/). |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } |  |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | Hämtar antalet bindningsrader i datakopplingsläge. |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | Hämtar eller anger DataMember från den flermedlems‑DataSource. Generellt representerar den ett DataTable‑objekt från ett DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | Hämtar eller anger DataSource. Vanligtvis är det ett DataSet-objekt. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | I data-binding-läge anger den om bindningskolumnrubriker ska skapas i bladet. |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | Hämtar HyperlinkCollection-samlingen. |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | Hämtar sitt eget index bland arbetsbladen. |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | Hämtar eller anger om arbetsbladet är skyddat. När ett arbetsblad är skyddat kan inte alla celler redigeras förutom den cell vars IsLocked‑egenskap är falsk. |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | Hämtar eller anger namnet på bladet. |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } |  |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | Hämtar datavalideringsinställningssamlingen i arbetsbladet. |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | Anger om detta bladnamn visas i bladflikarna i kontrollen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn)(int) | Anpassar automatiskt kolumnbredden. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Anpassar automatiskt kolumnbredden. Denna metod anpassar automatiskt en kolumn baserat på innehållet i ett cellintervall inom kolumnen från startRow till endRow. AutoFitColumn är en inexakt funktion. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | Avbryter och tar bort den nyligen tillagda bindningsraden. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | Bekräftar den nyligen tillagda bindningsraden och lägger till den i datakällan. |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | Kopierar från ett annat arbetsbladobjekt. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | Efter att ha ställt in en datasource för arbetsbladet, anropa den här metoden för att automatiskt generera bindningskolumnerna. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | Skapar en ny bindningsrad och binder den till datasource. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Skapar delsumma i bladet. |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | Bind bladet till DataSource. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | Tar bort en bindningsrad. |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | Fryser rutor vid den angivna cellen i kalkylbladet. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows)(int, int) | Grupperar rader. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows_1)(int, int, bool) | Grupperar rader. |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | Gör alla celler redigerbara. Detta är ett utökat attribut |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | Gör alla celler skrivskyddade. Detta är ett utökat attribut, observera att detta attribut inte kan behållas i den faktiska cellen; om du vill behålla skyddet, använd setProtect. |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | Gör ett område av celler redigerbara. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Gör alla celler skrivskyddade genom att anropa metoden SetAllCellsReadonly. Anropa sedan denna metod för att specificera vilka cellområden som ska vara redigerbara. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | Gör ett område av celler skrivskyddade. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Först gör alla celler redigerbara genom att anropa metoden SetAllCellsEditable. Anropa sedan denna metod för att specificera vilka cellområden som ska vara skrivskyddade. |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | Låser upp fönstren i kalkylbladet. |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | Avgrupperar rader. |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | Uppdaterar egenskapsvärdet för bindningsdatakällans post enligt cellens värde. |

### Anmärkningar

OBS: Denna klass är nu föråldrad. vänligen använd GridWorksheet istället. Klassen kommer att tas bort efter 6 månader från augusti 2014. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp

 [C#]
 ...
 using System.Web.UI.WebControls;
 ...
 ...

 WebWorksheets Worksheets = GridWeb1.WebWorksheets;
	WebCells cells = Worksheets[0].Cells;

	//Ställer in standardhöjd för rad
	cells.StandardHeight = new Unit(16, UnitType.Point);
	//Ställer in radens höjd
	cells.SetRowHeight(2, new Unit(20, UnitType.Point));

	//Ställer in standardbredd för kolumn
	cells.StandardWidth = new Unit(50, UnitType.Point);
	//Ställer in kolumnbredd
	cells.SetColumnWidth(3, new Unit(80, UnitType.Point));

	//Sammanfoga celler
	cells.Merge(5, 4, 2, 2);

	//Importera data
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

 //Importera från Excel-fil
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

### Se även

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)



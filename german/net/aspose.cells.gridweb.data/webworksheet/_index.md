---
title: "Klasse WebWorksheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.WebWorksheet Klasse. Stellt ein Web‑Arbeitsblatt dar."
type: docs
url: /de/net/aspose.cells.gridweb.data/webworksheet/
---
## WebWorksheet class

Stellt ein Web-Arbeitsblatt dar.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet instead")]
public class WebWorksheet : Control, ISerializable
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [WebWorksheet](webworksheet/#constructor)() | Der Konstruktor von WebWorksheet. |
| [WebWorksheet](webworksheet/#constructor_1)(MainWeb, GridWorksheet) | Der Konstruktor von WebWorksheet. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | Binden Sie die Spaltensammlung. |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | Das tatsächlich zur Laufzeit bindende Datenquellenobjekt. Es ist ein DataView-Objekt, wenn die DataSource-Eigenschaft ein DataSet-, DataTable- oder DataView-Objekt ist. |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | Im Datenbindungsmodus geben BindStartRow und BindStartColumn die Position des Rasters an, das an die Datenquelle gebunden werden soll. |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | Im Datenbindungsmodus geben BindStartRow und BindStartColumn die Position des Rasters an, das an die Datenquelle gebunden werden soll. |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } |  |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | Liefert die [`WebCells`](../webcells/). |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } |  |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | Liefert die Anzahl der Bindungszeilen im Datenbindungsmodus. |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | Liest oder setzt das DataMember der mehrgliedrigen DataSource. Im Allgemeinen stellt es ein DataTable-Objekt eines DataSet dar. |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | Liest oder setzt die DataSource. Im Allgemeinen ist es ein DataSet-Objekt. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | Im Datenbindungsmodus gibt an, ob Spaltenkopfbeschriftungen im Blatt erstellt werden sollen. |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | Liefert die HyperlinkCollection‑Sammlung. |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | Liefert den Index von sich selbst innerhalb der Arbeitsblätter. |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | Liest oder setzt, ob das Arbeitsblatt geschützt ist. Wenn ein Arbeitsblatt geschützt ist, können alle Zellen nicht bearbeitet werden, außer der Zelle, deren IsLocked‑Eigenschaft false ist. |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | Liest oder setzt den Namen des Blatts. |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } |  |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | Ruft die Datengültigkeits‑Einstellungs‑Sammlung im Arbeitsblatt ab. |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | Gibt an, ob der Name dieses Blatts in den Blattregisterkarten der Steuerung angezeigt wird. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn)(int) | Passt die Spaltenbreite automatisch an. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Passt die Spaltenbreite automatisch an. Diese Methode passt eine Spalte anhand des Inhalts in einem Zellbereich innerhalb der Spalte von startRow bis endRow automatisch an. AutoFitColumn ist eine ungenaue Funktion. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | Bricht ab und löscht die neu hinzugefügte Bindungszeile. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | Bestätigt die neu hinzugefügte Bindungszeile und fügt sie der Datenquelle hinzu. |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | Kopiert von einem anderen Arbeitsblatt‑Objekt. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | Nachdem eine Datenquelle für das Arbeitsblatt festgelegt wurde, rufen Sie diese Methode auf, um die Bindungsspalten automatisch zu erzeugen. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | Erstellt eine neue Bindungszeile und bindet sie an die Datenquelle. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Erstellt eine Zwischensumme im Blatt. |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | Bindet das Blatt an die DataSource. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | Löscht eine Bindungszeile. |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | Friert die Bildschirmelemente an der angegebenen Zelle im Arbeitsblatt ein. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows)(int, int) | Gruppiert Zeilen. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows_1)(int, int, bool) | Gruppiert Zeilen. |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | Macht alle Zellen editierbar. Dies ist ein erweitertes Attribut. |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | Macht alle Zellen schreibgeschützt. Dies ist ein erweitertes Attribut; beachten Sie, dass dieses Attribut in der tatsächlichen Zelle nicht beibehalten wird. Wenn Sie den Schutz beibehalten möchten, verwenden Sie bitte setProtect. |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | Macht einen Zellbereich editierbar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Macht alle Zellen schreibgeschützt, indem die Methode SetAllCellsReadonly aufgerufen wird. Rufen Sie anschließend diese Methode auf, um den Zellbereich festzulegen, der editierbar sein soll. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | Macht einen Zellbereich schreibgeschützt. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Zuerst alle Zellen editierbar machen, indem die Methode SetAllCellsEditable aufgerufen wird. Dann diese Methode aufrufen, um den Zellbereich festzulegen, der schreibgeschützt sein soll. |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | Löst das Einfrieren von Bereichen im Arbeitsblatt auf. |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | Löst die Gruppierung von Zeilen auf. |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | Aktualisiert den Eigenschaftswert des Bindungs‑Datenquellen‑Datensatzes gemäß dem Zellenwert. |

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Bitte verwenden Sie stattdessen GridWorksheet. Diese Klasse wird nach 6 Monaten ab August 2014 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben könnten.

### Beispiele

```csharp

 [C#]
 ...
 using System.Web.UI.WebControls;
 ...
 ...

 WebWorksheets Worksheets = GridWeb1.WebWorksheets;
	WebCells cells = Worksheets[0].Cells;

	//Setzt die Standardzeilenhöhe
	cells.StandardHeight = new Unit(16, UnitType.Point);
	//Setzt die Zeilenhöhe
	cells.SetRowHeight(2, new Unit(20, UnitType.Point));

	//Setzt die Standardspaltenbreite
	cells.StandardWidth = new Unit(50, UnitType.Point);
	//Setzt die Spaltenbreite
	cells.SetColumnWidth(3, new Unit(80, UnitType.Point));

	//Zellen zusammenführen
	cells.Merge(5, 4, 2, 2);

	//Daten importieren
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

 //Aus Excel‑Datei importieren
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

### Siehe auch

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)



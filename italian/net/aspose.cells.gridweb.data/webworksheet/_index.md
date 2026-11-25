---
title: "Classe WebWorksheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Data.WebWorksheet. Rappresenta un foglio di lavoro web"
type: docs
url: /it/net/aspose.cells.gridweb.data/webworksheet/
---
## WebWorksheet class

Rappresenta un foglio di lavoro web.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet instead")]
public class WebWorksheet : Control, ISerializable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WebWorksheet](webworksheet/#constructor)() | Il costruttore di WebWorksheet. |
| [WebWorksheet](webworksheet/#constructor_1)(MainWeb, GridWorksheet) | Il costruttore di WebWorksheet. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | Associa la raccolta di colonne. |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | L'oggetto datasource effettivamente associato a runtime. È un oggetto DataView quando la proprietà DataSource è un oggetto DataSet, DataTable o DataView. |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | In modalità data-binding, BindStartRow e BindStartColumn indicano la posizione della griglia da associare al datasource. |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | In modalità data-binding, BindStartRow e BindStartColumn indicano la posizione della griglia da associare al datasource. |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } |  |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | Ottiene i [`WebCells`](../webcells/). |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } |  |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | Ottiene il numero di righe di binding in modalità data-binding. |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | Ottiene o imposta il DataMember dal DataSource multivalore. Generalmente rappresenta un oggetto DataTable di un DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | Ottiene o imposta il DataSource. Generalmente è un oggetto DataSet. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | In modalità data-binding, indica se creare le didascalie delle intestazioni di colonna di binding nel foglio. |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | Ottiene la collezione HyperlinkCollection. |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | Ottiene l'indice di sé stesso all'interno dei fogli di lavoro. |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | Ottiene o imposta se il foglio di lavoro è protetto. Quando un foglio di lavoro è protetto, tutte le celle non possono essere modificate eccetto quelle la cui proprietà IsLocked è false. |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | Ottiene o imposta il nome del foglio. |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } |  |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | Ottiene la collezione delle impostazioni di convalida dei dati nel foglio di lavoro. |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | Indica se il nome di questo foglio è mostrato nelle schede del foglio del controllo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn)(int) | Adatta automaticamente la larghezza della colonna. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Adatta automaticamente la larghezza della colonna. Questo metodo adatta automaticamente una colonna in base al contenuto di un intervallo di celle nella colonna da startRow a endRow. AutoFitColumn è una funzione imprecisa. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | Annulla ed elimina la nuova riga di binding aggiunta. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | Conferma la nuova riga di binding aggiunta e la aggiunge al datasource. |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | Copia da un altro oggetto foglio di lavoro. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | Dopo aver impostato un datasource per il foglio di lavoro, chiama questo metodo per generare automaticamente le colonne di binding. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | Crea una nuova riga di binding e la associa al datasource. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Crea un subtotale nel foglio. |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | Associa il foglio al DataSource. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | Elimina una riga di binding. |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | Blocca i riquadri nella cella specificata nel foglio di lavoro. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows)(int, int) | Raggruppa le righe. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows_1)(int, int, bool) | Raggruppa le righe. |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | Rende tutte le celle modificabili. questo è un attributo esteso |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | Rende tutte le celle di sola lettura. questo è un attributo esteso, nota che questo attributo non può essere mantenuto nella cella reale; se desideri mantenere la protezione, usa setProtect |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | Rende modificabile un intervallo di celle. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Rendi tutte le celle di sola lettura chiamando il metodo SetAllCellsReadonly. poi chiama questo metodo per specificare l'intervallo di celle da rendere modificabile |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | Rende un intervallo di celle di sola lettura. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Prima rendi tutte le celle modificabili chiamando il metodo SetAllCellsEditable. poi chiama questo metodo per specificare l'intervallo di celle da rendere di sola lettura |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | Sblocca i riquadri nel worksheet. |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | Separa le righe dal raggruppamento. |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | Aggiorna il valore della proprietà del record della sorgente dati di binding in base al valore della cella. |

### Osservazioni

NOTA: Questa classe è ora obsoleta. Si prega di utilizzare GridWorksheet invece. Questa classe sarà rimossa dopo 6 mesi da agosto 2014. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp

 [C#]
 ...
 using System.Web.UI.WebControls;
 ...
 ...

 WebWorksheets Worksheets = GridWeb1.WebWorksheets;
	WebCells cells = Worksheets[0].Cells;

	//Imposta l'altezza predefinita della riga
	cells.StandardHeight = new Unit(16, UnitType.Point);
	//Imposta l'altezza della riga
	cells.SetRowHeight(2, new Unit(20, UnitType.Point));

	//Imposta la larghezza predefinita della colonna
	cells.StandardWidth = new Unit(50, UnitType.Point);
	//Imposta la larghezza della colonna
	cells.SetColumnWidth(3, new Unit(80, UnitType.Point));

	//Unisci le celle
	cells.Merge(5, 4, 2, 2);

	//Importa dati
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

 //Importa da file Excel
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

### Vedi anche

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)



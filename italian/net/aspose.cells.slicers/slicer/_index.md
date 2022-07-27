---
title: Slicer
second_title: Riferimento alle API di Aspose.Cells per .NET
description: descrizione sommaria di Slicer View
type: docs
weight: 5630
url: /it/net/aspose.cells.slicers/slicer/
---
## Slicer class

descrizione sommaria di Slicer View

```csharp
public class Slicer
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AlternativeText](../../aspose.cells.slicers/slicer/alternativetext) { get; set; } | Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto Slicer. |
| [Caption](../../aspose.cells.slicers/slicer/caption) { get; set; } | Restituisce o imposta la didascalia dell'affettatrice specificata. |
| [CaptionVisible](../../aspose.cells.slicers/slicer/captionvisible) { get; set; } | Restituisce o imposta se l'intestazione che visualizza l'affettatrice Didascalia è visibile il valore predefinito è true |
| [ColumnWidth](../../aspose.cells.slicers/slicer/columnwidth) { get; set; } | Restituisce o imposta la larghezza, in punti, di ciascuna colonna nell'affettatrice. |
| [ColumnWidthPixel](../../aspose.cells.slicers/slicer/columnwidthpixel) { get; set; } | Ottiene o imposta la larghezza in unità di pixel per ciascuna colonna dello slicer. |
| [Height](../../aspose.cells.slicers/slicer/height) { get; set; } | Restituisce o imposta l'altezza dell'affettatrice specificata, in punti. |
| [HeightPixel](../../aspose.cells.slicers/slicer/heightpixel) { get; set; } | Restituisce o imposta l'altezza dello slicer specificato, in pixel. |
| [IsLocked](../../aspose.cells.slicers/slicer/islocked) { get; set; } | Indica se la forma dell'affettatrice è bloccata. |
| [IsPrintable](../../aspose.cells.slicers/slicer/isprintable) { get; set; } | Indica se l'oggetto slicer è stampabile. |
| [LeftPixel](../../aspose.cells.slicers/slicer/leftpixel) { get; set; } | Restituisce o imposta l'offset orizzontale della forma affettatrice dalla colonna di sinistra, in pixel. |
| [LockedAspectRatio](../../aspose.cells.slicers/slicer/lockedaspectratio) { get; set; } | Indica se bloccare le proporzioni. |
| [LockedPosition](../../aspose.cells.slicers/slicer/lockedposition) { get; set; } | Indica se lo slicer specificato può essere spostato o ridimensionato utilizzando l'interfaccia utente. |
| [Name](../../aspose.cells.slicers/slicer/name) { get; set; } | Restituisce o imposta il nome dell'affettatrice specificata |
| [NumberOfColumns](../../aspose.cells.slicers/slicer/numberofcolumns) { get; set; } | Restituisce o imposta il numero di colonne nello slicer specificato. |
| [Parent](../../aspose.cells.slicers/slicer/parent) { get; } | Restituisce l'oggetto Foglio di lavoro che rappresenta il foglio che contiene lo slicer. Sola lettura. |
| [Placement](../../aspose.cells.slicers/slicer/placement) { get; set; } | Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti. La proprietà controlla il posizionamento di un oggetto su un foglio di lavoro. |
| [RowHeight](../../aspose.cells.slicers/slicer/rowheight) { get; set; } | Restituisce o imposta l'altezza, in punti, di ogni riga nell'affettatrice specificata. |
| [RowHeightPixel](../../aspose.cells.slicers/slicer/rowheightpixel) { get; set; } | Restituisce o imposta l'altezza, in pixel, di ogni riga nello slicer specificato. |
| [SlicerCache](../../aspose.cells.slicers/slicer/slicercache) { get; } | Restituisce l'oggetto SlicerCache associato allo slicer. Sola lettura. |
| [StyleType](../../aspose.cells.slicers/slicer/styletype) { get; set; } | Specifica il tipo di stile affettatrice incorporata il tipo predefinito è SlicerStyleLight1 |
| [Title](../../aspose.cells.slicers/slicer/title) { get; set; } | Specifica il titolo dell'oggetto Slicer corrente. |
| [TopPixel](../../aspose.cells.slicers/slicer/toppixel) { get; set; } | Restituisce o imposta l'offset verticale della forma affettatrice dalla riga superiore, in pixel. |
| [Width](../../aspose.cells.slicers/slicer/width) { get; set; } | Restituisce o imposta la larghezza dell'affettatrice specificata, in punti. |
| [WidthPixel](../../aspose.cells.slicers/slicer/widthpixel) { get; set; } | Restituisce o imposta la larghezza dell'affettatrice specificata, in pixel. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddPivotConnection](../../aspose.cells.slicers/slicer/addpivotconnection)(PivotTable) | Aggiunge la connessione alla tabella pivot. |
| [Refresh](../../aspose.cells.slicers/slicer/refresh)() | Aggiornamento dell'affettatrice. Nel frattempo, aggiornamento e calcolo delle tabelle pivot relative. |
| [RemovePivotConnection](../../aspose.cells.slicers/slicer/removepivotconnection)(PivotTable) | Rimuove la connessione alla tabella pivot. |

### Esempi

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
pivot.RefreshData();
pivot.CalculateData();

SlicerCollection slicers = sheet.Slicers;
int slicerIndex = slicers.Add(pivot, "E12", "fruit");
Slicer slicer = slicers[slicerIndex];
slicer.StyleType = SlicerStyleType.SlicerStyleLight2;

SlicerCacheItemCollection items = slicer.SlicerCache.SlicerCacheItems;
SlicerCacheItem item = items[0];
item.Selected = false;
//fai i tuoi affari
book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10
pivot.RefreshData()
pivot.CalculateData()

Dim slicers As SlicerCollection = sheet.Slicers
Dim slicerIndex As Int32 = slicers.Add(pivot, "E12", "fruit")
Dim slicer As Slicer = slicers(slicerIndex)
slicer.StyleType = SlicerStyleType.SlicerStyleLight2

Dim items As SlicerCacheItemCollection = slicer.SlicerCache.SlicerCacheItems
Dim item As SlicerCacheItem = items(0)
item.Selected = False

book.Save("out_vb.xlsx")
```

### Guarda anche

* spazio dei nomi [Aspose.Cells.Slicers](../../aspose.cells.slicers)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

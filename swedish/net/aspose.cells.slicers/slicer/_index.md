---
title: Slicer
second_title: Aspose.Cells för .NET API-referens
description: sammanfattande beskrivning av Slicer View
type: docs
weight: 5630
url: /sv/net/aspose.cells.slicers/slicer/
---
## Slicer class

sammanfattande beskrivning av Slicer View

```csharp
public class Slicer
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AlternativeText](../../aspose.cells.slicers/slicer/alternativetext) { get; set; } | Returnerar eller ställer in den beskrivande (alternativa) textsträngen för Slicer-objektet. |
| [Caption](../../aspose.cells.slicers/slicer/caption) { get; set; } | Returnerar eller ställer in bildtexten för den angivna skivaren. |
| [CaptionVisible](../../aspose.cells.slicers/slicer/captionvisible) { get; set; } | Returnerar eller ställer in om rubriken som visar slicer Caption är visible standardvärdet är true |
| [ColumnWidth](../../aspose.cells.slicers/slicer/columnwidth) { get; set; } | Returnerar eller ställer in bredden, i punkter, för varje kolumn i utsnittet. |
| [ColumnWidthPixel](../../aspose.cells.slicers/slicer/columnwidthpixel) { get; set; } | Hämtar eller ställer in bredden i pixelenhet för varje kolumn i utsnittet. |
| [Height](../../aspose.cells.slicers/slicer/height) { get; set; } | Returnerar eller ställer in höjden på den angivna skivaren, i punkter. |
| [HeightPixel](../../aspose.cells.slicers/slicer/heightpixel) { get; set; } | Returnerar eller ställer in höjden på det angivna utsnittet i pixlar. |
| [IsLocked](../../aspose.cells.slicers/slicer/islocked) { get; set; } | Indikerar om skärformen är låst. |
| [IsPrintable](../../aspose.cells.slicers/slicer/isprintable) { get; set; } | Indikerar om skivobjektet är utskrivbart. |
| [LeftPixel](../../aspose.cells.slicers/slicer/leftpixel) { get; set; } | Returnerar eller ställer in den horisontella förskjutningen av utsnittsformen från dess vänstra kolumn, i pixlar. |
| [LockedAspectRatio](../../aspose.cells.slicers/slicer/lockedaspectratio) { get; set; } | Indikerar om låsning av bildförhållande. |
| [LockedPosition](../../aspose.cells.slicers/slicer/lockedposition) { get; set; } | Indikerar om den angivna slicern kan flyttas eller storleksändras med hjälp av användargränssnittet. |
| [Name](../../aspose.cells.slicers/slicer/name) { get; set; } | Returnerar eller anger namnet på den angivna slicer |
| [NumberOfColumns](../../aspose.cells.slicers/slicer/numberofcolumns) { get; set; } | Returnerar eller ställer in antalet kolumner i det angivna utsnittet. |
| [Parent](../../aspose.cells.slicers/slicer/parent) { get; } | Returnerar kalkylbladsobjektet som representerar arket som innehåller utsnittet. Skrivskyddad. |
| [Placement](../../aspose.cells.slicers/slicer/placement) { get; set; } | Representerar hur ritobjektet är fäst vid cellerna under det. Egenskapen styr placeringen av ett objekt på ett kalkylblad. |
| [RowHeight](../../aspose.cells.slicers/slicer/rowheight) { get; set; } | Returnerar eller ställer in höjden, i poäng, för varje rad i den angivna slicern. |
| [RowHeightPixel](../../aspose.cells.slicers/slicer/rowheightpixel) { get; set; } | Returnerar eller ställer in höjden, i pixlar, för varje rad i det angivna utsnittet. |
| [SlicerCache](../../aspose.cells.slicers/slicer/slicercache) { get; } | Returnerar SlicerCache-objektet som är associerat med slicern. Skrivskyddad. |
| [StyleType](../../aspose.cells.slicers/slicer/styletype) { get; set; } | Ange typen av inbyggd slicer style standardtypen är SlicerStyleLight1 |
| [Title](../../aspose.cells.slicers/slicer/title) { get; set; } | Anger titeln på det aktuella Slicer-objektet. |
| [TopPixel](../../aspose.cells.slicers/slicer/toppixel) { get; set; } | Returnerar eller ställer in den vertikala förskjutningen av utsnittsformen från dess översta raden, i pixlar. |
| [Width](../../aspose.cells.slicers/slicer/width) { get; set; } | Returnerar eller ställer in bredden på den angivna skivaren, i punkter. |
| [WidthPixel](../../aspose.cells.slicers/slicer/widthpixel) { get; set; } | Returnerar eller ställer in bredden på det angivna utsnittet i pixlar. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [AddPivotConnection](../../aspose.cells.slicers/slicer/addpivotconnection)(PivotTable) | Lägger till pivottabellanslutning. |
| [Refresh](../../aspose.cells.slicers/slicer/refresh)() | Uppdaterar skivaren. Under tiden uppdaterar och beräknar relativa pivottabeller. |
| [RemovePivotConnection](../../aspose.cells.slicers/slicer/removepivotconnection)(PivotTable) | Tar bort PivotTable-anslutning. |

### Exempel

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
//gör dina affärer
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

### Se även

* namnutrymme [Aspose.Cells.Slicers](../../aspose.cells.slicers)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

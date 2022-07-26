---
title: Slicer
second_title: Aspose.Cells für .NET-API-Referenz
description: zusammenfassende Beschreibung der Slicer-Ansicht
type: docs
weight: 5630
url: /de/net/aspose.cells.slicers/slicer/
---
## Slicer class

zusammenfassende Beschreibung der Slicer-Ansicht

```csharp
public class Slicer
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AlternativeText](../../aspose.cells.slicers/slicer/alternativetext) { get; set; } | Gibt die beschreibende (alternative) Textzeichenfolge des Slicer-Objekts zurück oder legt sie fest. |
| [Caption](../../aspose.cells.slicers/slicer/caption) { get; set; } | Gibt die Beschriftung des angegebenen Slicers zurück oder legt sie fest. |
| [CaptionVisible](../../aspose.cells.slicers/slicer/captionvisible) { get; set; } | Gibt zurück oder legt fest, ob der Header, der die Slicer-Beschriftung anzeigt, sichtbar ist der Standardwert ist true |
| [ColumnWidth](../../aspose.cells.slicers/slicer/columnwidth) { get; set; } | Gibt die Breite jeder Spalte im Slicer in Punkt zurück oder legt sie fest. |
| [ColumnWidthPixel](../../aspose.cells.slicers/slicer/columnwidthpixel) { get; set; } | Ruft die Breite in Pixeleinheiten für jede Spalte des Slicers ab oder legt sie fest. |
| [Height](../../aspose.cells.slicers/slicer/height) { get; set; } | Gibt die Höhe des angegebenen Slicers in Punkt zurück oder legt sie fest. |
| [HeightPixel](../../aspose.cells.slicers/slicer/heightpixel) { get; set; } | Gibt die Höhe des angegebenen Slicers in Pixel zurück oder legt sie fest. |
| [IsLocked](../../aspose.cells.slicers/slicer/islocked) { get; set; } | Gibt an, ob die Slicer-Form gesperrt ist. |
| [IsPrintable](../../aspose.cells.slicers/slicer/isprintable) { get; set; } | Gibt an, ob das Slicer-Objekt druckbar ist. |
| [LeftPixel](../../aspose.cells.slicers/slicer/leftpixel) { get; set; } | Gibt den horizontalen Versatz der Slicer-Form von der linken Spalte in Pixel zurück oder legt ihn fest. |
| [LockedAspectRatio](../../aspose.cells.slicers/slicer/lockedaspectratio) { get; set; } | Gibt an, ob das Seitenverhältnis gesperrt wird. |
| [LockedPosition](../../aspose.cells.slicers/slicer/lockedposition) { get; set; } | Gibt an, ob der angegebene Slicer mithilfe der Benutzeroberfläche verschoben oder in der Größe geändert werden kann. |
| [Name](../../aspose.cells.slicers/slicer/name) { get; set; } | Gibt den Namen des angegebenen Slicer zurück oder legt ihn fest |
| [NumberOfColumns](../../aspose.cells.slicers/slicer/numberofcolumns) { get; set; } | Gibt die Anzahl der Spalten im angegebenen Slicer zurück oder legt sie fest. |
| [Parent](../../aspose.cells.slicers/slicer/parent) { get; } | Gibt das Worksheet-Objekt zurück, das das Blatt darstellt, das den Slicer enthält. Schreibgeschützt. |
| [Placement](../../aspose.cells.slicers/slicer/placement) { get; set; } | Stellt dar, wie das Zeichnungsobjekt an die darunter liegenden Zellen angehängt ist. Die Eigenschaft steuert die Platzierung eines Objekts auf einem Arbeitsblatt. |
| [RowHeight](../../aspose.cells.slicers/slicer/rowheight) { get; set; } | Gibt die Höhe jeder Zeile im angegebenen Slicer in Punkt zurück oder legt sie fest. |
| [RowHeightPixel](../../aspose.cells.slicers/slicer/rowheightpixel) { get; set; } | Gibt die Höhe jeder Zeile im angegebenen Slicer in Pixel zurück oder legt sie fest. |
| [SlicerCache](../../aspose.cells.slicers/slicer/slicercache) { get; } | Gibt das dem Slicer zugeordnete SlicerCache-Objekt zurück. Schreibgeschützt. |
| [StyleType](../../aspose.cells.slicers/slicer/styletype) { get; set; } | Geben Sie den Typ des integrierten Slicer-Stils an Der Standardtyp ist SlicerStyleLight1 |
| [Title](../../aspose.cells.slicers/slicer/title) { get; set; } | Gibt den Titel des aktuellen Slicer-Objekts an. |
| [TopPixel](../../aspose.cells.slicers/slicer/toppixel) { get; set; } | Gibt den vertikalen Versatz der Slicer-Form von der obersten Zeile in Pixel zurück oder legt ihn fest. |
| [Width](../../aspose.cells.slicers/slicer/width) { get; set; } | Gibt die Breite des angegebenen Slicers in Punkt zurück oder legt sie fest. |
| [WidthPixel](../../aspose.cells.slicers/slicer/widthpixel) { get; set; } | Gibt die Breite des angegebenen Slicers in Pixel zurück oder legt sie fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddPivotConnection](../../aspose.cells.slicers/slicer/addpivotconnection)(PivotTable) | Fügt eine PivotTable-Verbindung hinzu. |
| [Refresh](../../aspose.cells.slicers/slicer/refresh)() | Aktualisieren des Slicers. In der Zwischenzeit Aktualisieren und Berechnen relativer PivotTables. |
| [RemovePivotConnection](../../aspose.cells.slicers/slicer/removepivotconnection)(PivotTable) | Entfernt die PivotTable-Verbindung. |

### Beispiele

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
// Mach dein Geschäft
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

### Siehe auch

* namensraum [Aspose.Cells.Slicers](../../aspose.cells.slicers)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

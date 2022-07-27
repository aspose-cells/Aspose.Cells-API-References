---
title: DataBar
second_title: Aspose.Cells für .NET-API-Referenz
description: Beschreiben Sie die bedingte DataBar-Formatierungsregel. Diese Regel zur bedingten Formatierung zeigt einen abgestuften Datenbalken im Zellbereich an.
type: docs
weight: 1240
url: /de/net/aspose.cells/databar/
---
## DataBar class

Beschreiben Sie die bedingte DataBar-Formatierungsregel. Diese Regel zur bedingten Formatierung zeigt einen abgestuften Datenbalken im Zellbereich an.

```csharp
public class DataBar
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor) { get; set; } | Ruft die Farbe der Achse für Zellen mit bedingter Formatierung als Datenbalken ab. |
| [AxisPosition](../../aspose.cells/databar/axisposition) { get; set; } | Ruft die Position der Achse der Datenbalken ab oder legt sie fest, die durch eine bedingte Formatierungsregel angegeben ist. |
| [BarBorder](../../aspose.cells/databar/barborder) { get; } | Ruft ein Objekt ab, das den Rahmen eines Datenbalkens angibt. |
| [BarFillType](../../aspose.cells/databar/barfilltype) { get; set; } | Ruft ab oder legt fest, wie ein Datenbalken mit Farbe gefüllt wird. |
| [Color](../../aspose.cells/databar/color) { get; set; } | Holen oder setzen Sie die Farbe dieses DataBar. |
| [Direction](../../aspose.cells/databar/direction) { get; set; } | Ruft die Richtung ab, in der die Datenleiste angezeigt wird, oder legt sie fest. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo) { get; } | Abrufen oder Festlegen des Maximalwertobjekts dieses DataBar. Kann null oder CFValueObject mit dem Typ FormatConditionValueType.Min nicht darauf festlegen. |
| [MaxLength](../../aspose.cells/databar/maxlength) { get; set; } | Repräsentiert die maximale Länge des Datenbalkens. |
| [MinCfvo](../../aspose.cells/databar/mincfvo) { get; } | Abrufen oder Festlegen des Mindestwertobjekts dieses DataBar. Kann null oder CFValueObject mit dem Typ FormatConditionValueType.Max nicht darauf festlegen. |
| [MinLength](../../aspose.cells/databar/minlength) { get; set; } | Repräsentiert die Mindestlänge des Datenbalkens. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat) { get; } | Ruft das NegativeBarFormat-Objekt ab, das einer bedingten Formatierungsregel für Datenbalken zugeordnet ist. |
| [ShowValue](../../aspose.cells/databar/showvalue) { get; set; } | Holen oder setzen Sie das Flag, das angibt, ob die Werte der Zellen angezeigt werden sollen, auf die dieser Datenbalken angewendet wird. Der Standardwert ist wahr. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage)(Cell, ImageOrPrintOptions) | Renderdatenbalken in Zelle zu Bild-Byte-Array. |

### Beispiele

```csharp

[C#]

//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

//Fügt eine leere bedingte Formatierung hinzu
int index = sheet.ConditionalFormattings.Add();

FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

//Legt den bedingten Formatbereich fest.
CellArea ca = new CellArea();

ca.StartRow = 0;

ca.EndRow = 2;

ca.StartColumn = 0;

ca.EndColumn = 0;

fcs.AddArea(ca);

//Bedingung hinzufügen.
int idx = fcs.AddCondition(FormatConditionType.DataBar);

fcs.AddArea(ca);

FormatCondition cond = fcs[idx];

//Databar abrufen
DataBar dataBar = cond.DataBar;

dataBar.Color = Color.Orange;

//Databar-Eigenschaften festlegen
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;

dataBar.MinCfvo.Value = 30;

dataBar.ShowValue = false;

dataBar.BarBorder.Type = DataBarBorderType.Solid;

dataBar.BarBorder.Color = Color.Plum;

 dataBar.BarFillType = DataBarFillType.Solid;
  
 dataBar.AxisColor = Color.Red;
 
 dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
 
 dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
 
 dataBar.NegativeBarFormat.Color = Color.White;
 
 dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
 
 dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
 
//Zellwerte setzen
Aspose.Cells.Cell cell1 = sheet.Cells["A1"];

cell1.PutValue(10);

Aspose.Cells.Cell cell2 = sheet.Cells["A2"];

cell2.PutValue(120);

Aspose.Cells.Cell cell3 = sheet.Cells["A3"];

cell3.PutValue(260);

//Speichern der Excel-Datei
workbook.Save("book1.xlsx");

[VB.NET]

'Instanziieren eines Workbook-Objekts
Dim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'Fügt eine leere bedingte Formatierung hinzu
Dim index As Integer = sheet.ConditionalFormattings.Add()

Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)

'Legt den bedingten Formatbereich fest.
Dim ca As New CellArea()

ca.StartRow = 0

ca.EndRow = 2

ca.StartColumn = 0

ca.EndColumn = 0

fcs.AddArea(ca)

'Fügt Bedingung hinzu.
Dim idx As Integer = fcs.AddCondition(FormatConditionType.DataBar)

fcs.AddArea(ca)

Dim cond As FormatCondition = fcs(idx)

'Holen Sie sich Databar
Dim dataBar As DataBar = cond.DataBar

dataBar.Color = Color.Orange

'Databar-Eigenschaften festlegen
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile

dataBar.MinCfvo.Value = 30

dataBar.ShowValue = False

dataBar.BarBorder.Type = DataBarBorderType.Solid

dataBar.BarBorder.Color = Color.Plum

 dataBar.BarFillType = DataBarFillType.Solid
  
 dataBar.AxisColor = Color.Red
 
 dataBar.AxisPosition = DataBarAxisPosition.Midpoint
 
 dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color
 
 dataBar.NegativeBarFormat.Color = Color.White
 
 dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color
 
 dataBar.NegativeBarFormat.BorderColor = Color.Yellow

'Zellenwerte setzen
Dim cell1 As Aspose.Cells.Cell = sheet.Cells("A1")

cell1.PutValue(10)

Dim cell2 As Aspose.Cells.Cell = sheet.Cells("A2")

cell2.PutValue(120)

Dim cell3 As Aspose.Cells.Cell = sheet.Cells("A3")

cell3.PutValue(260)

'Speichern der Excel-Datei
workbook.Save("book1.xlsx")

```

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

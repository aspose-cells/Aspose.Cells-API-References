---
title: DataBar
second_title: Aspose.Cells för .NET API-referens
description: Beskriv DataBars villkorliga formateringsregel. Denna regel för villkorlig formatering visar en gradated datafält i cellintervallet.
type: docs
weight: 1240
url: /sv/net/aspose.cells/databar/
---
## DataBar class

Beskriv DataBars villkorliga formateringsregel. Denna regel för villkorlig formatering visar en gradated datafält i cellintervallet.

```csharp
public class DataBar
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor) { get; set; } | Får färgen på axeln för celler med villkorlig formatering som datafält. |
| [AxisPosition](../../aspose.cells/databar/axisposition) { get; set; } | Hämtar eller ställer in positionen för axeln för datastaplarna som anges av en villkorlig formateringsregel. |
| [BarBorder](../../aspose.cells/databar/barborder) { get; } | Hämtar ett objekt som anger gränsen för ett datafält. |
| [BarFillType](../../aspose.cells/databar/barfilltype) { get; set; } | Hämtar eller ställer in hur ett datafält fylls med färg. |
| [Color](../../aspose.cells/databar/color) { get; set; } | Hämta eller ställ in denna DataBars färg. |
| [Direction](../../aspose.cells/databar/direction) { get; set; } | Hämtar eller ställer in riktningen som datafältet visas. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo) { get; } | Hämta eller ställ in denna DataBars maxvärdeobjekt. Kan inte ställa in null eller CFValueObject med typen FormatConditionValueType.Min till det. |
| [MaxLength](../../aspose.cells/databar/maxlength) { get; set; } | Representerar maxlängden på datafältet. |
| [MinCfvo](../../aspose.cells/databar/mincfvo) { get; } | Hämta eller ställ in denna DataBars minvärdeobjekt. Kan inte ställa in null eller CFValueObject med typen FormatConditionValueType.Max till det. |
| [MinLength](../../aspose.cells/databar/minlength) { get; set; } | Representerar den minsta längden på datafältet. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat) { get; } | Hämtar NegativeBarFormat-objektet som är kopplat till en regel för villkorlig formatering av datafält. |
| [ShowValue](../../aspose.cells/databar/showvalue) { get; set; } | Hämta eller ställ in flaggan som anger om värdena för cellerna som denna datafält används på ska visas. Standardvärdet är sant. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage)(Cell, ImageOrPrintOptions) | Rendera datafält i cell till bildbyte-array. |

### Exempel

```csharp

[C#]

//Instantiering av ett arbetsboksobjekt
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

//Lägger till en tom villkorlig formatering
int index = sheet.ConditionalFormattings.Add();

FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

//Ställer in det villkorliga formatintervallet.
CellArea ca = new CellArea();

ca.StartRow = 0;

ca.EndRow = 2;

ca.StartColumn = 0;

ca.EndColumn = 0;

fcs.AddArea(ca);

//Lägger till villkor.
int idx = fcs.AddCondition(FormatConditionType.DataBar);

fcs.AddArea(ca);

FormatCondition cond = fcs[idx];

//Hämta Databar
DataBar dataBar = cond.DataBar;

dataBar.Color = Color.Orange;

//Ange datafältsegenskaper
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
 
//Sätt cellvärden
Aspose.Cells.Cell cell1 = sheet.Cells["A1"];

cell1.PutValue(10);

Aspose.Cells.Cell cell2 = sheet.Cells["A2"];

cell2.PutValue(120);

Aspose.Cells.Cell cell3 = sheet.Cells["A3"];

cell3.PutValue(260);

//Spara Excel-filen
workbook.Save("book1.xlsx");

[VB.NET]

'Instantiera ett arbetsboksobjekt
Dim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'Lägger till en tom villkorlig formatering
Dim index As Integer = sheet.ConditionalFormattings.Add()

Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)

'Ställer in det villkorliga formatintervallet.
Dim ca As New CellArea()

ca.StartRow = 0

ca.EndRow = 2

ca.StartColumn = 0

ca.EndColumn = 0

fcs.AddArea(ca)

'Lägger till skick.
Dim idx As Integer = fcs.AddCondition(FormatConditionType.DataBar)

fcs.AddArea(ca)

Dim cond As FormatCondition = fcs(idx)

'Skaffa Databar
Dim dataBar As DataBar = cond.DataBar

dataBar.Color = Color.Orange

'Ställ in datafältsegenskaper
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

'Sätt cellvärden
Dim cell1 As Aspose.Cells.Cell = sheet.Cells("A1")

cell1.PutValue(10)

Dim cell2 As Aspose.Cells.Cell = sheet.Cells("A2")

cell2.PutValue(120)

Dim cell3 As Aspose.Cells.Cell = sheet.Cells("A3")

cell3.PutValue(260)

'Sparar Excel-filen
workbook.Save("book1.xlsx")

```

### Se även

* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

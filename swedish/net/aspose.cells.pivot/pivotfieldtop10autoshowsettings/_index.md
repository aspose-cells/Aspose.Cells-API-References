---
title: "Klass PivotFieldTop10AutoShowSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotFieldTop10AutoShowSettings-klass. Representerar Top 10 AutoShow-inställningarna för ett pivåfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldtop10autoshowsettings/
---
## PivotFieldTop10AutoShowSettings class

Representerar Top 10 AutoShow-inställningarna för ett pivottfält.

```csharp
public class PivotFieldTop10AutoShowSettings
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AutoShowCount](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/autoshowcount/) { get; set; } | Representerar antalet topp- eller bottenobjekt som automatiskt visas i det angivna pivåtabellfältet. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/isautoshow/) { get; set; } | Indikerar om ett "Top 10 AutoShow"-filter har tillämpats på detta fält. |
| [IsTop](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/istop/) { get; set; } | Indikerar om det angivna pivåtabellfältet automatiskt visas i stigande ordning. |
| [RankBy](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/rankby/) { get; set; } | Anger indexet för datafältet för AutoShow-rangordning. Representerar auto show-fältets index. -1 betyder PivotField själv. Det bör vara indexet för datafälten. |

### Anmärkningar

I xls: Implementering av topp‑10‑filter i Xls via Top 10 AutoShow. I ooxml‑filer: Det underliggande ooxml‑filformatet stöder Top10 AutoShow, men Excel 2007 och senare användargränssnitt ger endast åtkomst via Top10‑filter. Om XLS‑kompatibilitet inte krävs rekommenderas att använda Top10‑filter istället.

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

PivotTable pivot = pivots.Add("=Sheet1!A1:C9", "A12");

pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
           
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
           
 //Ändra attribut för PivotField
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

//Visa de två översta objekten efter radfältsetikett.
rowField.Top10AutoShow(true, true, 2, -1);

PivotFieldTop10AutoShowSettings sortSetting = rowField.Top10AutoShowSettings;
Console.WriteLine(sortSetting.IsAutoShow);

 pivot.CalculateData();

book.Save("out.xlsx");

[Visual Basic]

Dim book As New Workbook()
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

Dim pivot As PivotTable = pivots.Add("=Sheet1!A1:C9", "A12")
 
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
pivot.AddFieldToArea(PivotFieldType.Column, "year")
pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'Show top 2 items by row field label.
rowField.Top10AutoShow(True, True, 2, -1)

Dim sortSetting As PivotFieldTop10AutoShowSettings = rowField.Top10AutoShowSettings
Console.WriteLine(sortSetting.IsAutoShow)

pivot.CalculateData()

book.Save("out.xlsx")
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)



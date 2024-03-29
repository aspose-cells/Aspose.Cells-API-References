---
title: ChartPointCollection
second_title: Aspose.Cells för .NET API-referens
description: Representerar en samling som innehåller alla punkter i en serie.
type: docs
weight: 520
url: /sv/net/aspose.cells.charts/chartpointcollection/
---
## ChartPointCollection class

Representerar en samling som innehåller alla punkter i en serie.

```csharp
public class ChartPointCollection
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Count](../../aspose.cells.charts/chartpointcollection/count) { get; } | Får räkningen av diagrampunkten. |
| [Item](../../aspose.cells.charts/chartpointcollection/item) { get; } | Får[`ChartPoint`](../chartpoint) element vid det angivna indexet i serien. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Clear](../../aspose.cells.charts/chartpointcollection/clear)() | Ta bort alla inställningar för sjökortspunkterna. |
| [GetEnumerator](../../aspose.cells.charts/chartpointcollection/getenumerator)() | Returnerar en uppräkning för hela[`ChartPointCollection`](../chartpointcollection) . |
| [RemoveAt](../../aspose.cells.charts/chartpointcollection/removeat)(int) | Tar bort punkt vid indexet för serien.. |

### Exempel

```csharp
//Instantiering av ett arbetsboksobjekt
Workbook workbook = new Workbook();

//Hämta referensen till det första kalkylbladet
Worksheet worksheet = workbook.Worksheets[0];

//Lägga till ett exempelvärde i cellen "A1".
worksheet.Cells["A1"].PutValue(50);

//Lägga till ett exempelvärde till "A2"-cellen
worksheet.Cells["A2"].PutValue(100);

//Lägga till ett exempelvärde till "A3"-cellen
worksheet.Cells["A3"].PutValue(150);

//Lägga till ett exempelvärde till "B1"-cellen
worksheet.Cells["B1"].PutValue(60);

//Lägga till ett exempelvärde till "B2"-cellen
worksheet.Cells["B2"].PutValue(32);

//Lägga till ett exempelvärde till "B3"-cellen
worksheet.Cells["B3"].PutValue(50);

//Lägga till ett diagram i arbetsbladet
int chartIndex = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10);

//Åtkomst till instansen av det nyligen tillagda diagrammet
Chart chart = worksheet.Charts[chartIndex];

//Lägga till NSeries (diagramdatakälla) till diagrammet som sträcker sig från "A1"-cell till "B3"
chart.NSeries.Add("A1:B3", true);

//Visa dataetiketter 
chart.NSeries[0].DataLabels.IsValueShown = true;

ChartPointCollection points = chart.NSeries[0].Points;

for (int i = 0; i < points.Count; i++)
{
    //Hämta datapunkt
    ChartPoint point = points[i];
    //Set Pir Explosion
    point.Explosion = 15;
    //Ange kantfärg
    point.Border.Color = System.Drawing.Color.Red;
}

//Spara Excel-filen
workbook.Save("book1.xls");

[VB.NET]

'Instantiera ett arbetsboksobjekt
Dim workbook As Workbook = New Workbook()

'Få referensen till det första arbetsbladet
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)

'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)

'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)

'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)

'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)

'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)

'Lägga till ett diagram i arbetsbladet
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10)

'Åtkomst till instansen av det nyligen tillagda diagrammet
Dim chart As Chart = worksheet.Charts(chartIndex)

'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)

'Visa dataetiketter 
chart.NSeries(0).DataLabels.IsValueShown = True

Dim points As ChartPointCollection = chart.NSeries(0).Points

For i As Integer = 0 To points.Count - 1
    'Hämta datapunkt
    Dim point As ChartPoint = points(i)
    'Ställ Pir Explosion
    point.Explosion = 15
    'Ställ in kantfärg
    point.Border.Color = System.Drawing.Color.Red
Next i

'Sparar Excel-filen
workbook.Save("book1.xls")

```

### Se även

* namnutrymme [Aspose.Cells.Charts](../../aspose.cells.charts)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

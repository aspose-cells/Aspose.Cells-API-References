---
title: "SparklineCollection.Remove"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineCollection-metod. Tar bort sparkline"
type: docs
url: /sv/net/aspose.cells.charts/sparklinecollection/remove/
---
## SparklineCollection.Remove method

Tar bort sparkline

```csharp
[Obsolete("Use SparklineCollection.RemoveSparkline(Sparkline) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Remove(object o)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | Object |  |

### Anmärkningar

OBS: Den här medlemmen är nu föråldrad. Använd istället metoden RemoveSparkline(). Denna metod kommer att tas bort 6 månader senare från och med december 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineCollectionMethodRemoveWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Infoga exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);


            // Definiera CellArea där sparklines kommer att läggas till
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };

            // Lägg till en ny SparklineGroup i kalkylbladet
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];

            SparklineCollection sparklineCollection = sparklineGroup.Sparklines;

            // Lägg till sparklines i SparklineGroup
            sparklineCollection.Add("A1:D1", 0, 5);

            Console.WriteLine("Sparkline count: " + sparklineCollection.Count);

            // Ställ in olika egenskaper för SparklineGroup
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;

            // Ställ in färger för höga och låga punkter
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = System.Drawing.Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = System.Drawing.Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Ställ in seriefärgen och linjebredden
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = System.Drawing.Color.Orange;
            sparklineGroup.SeriesColor = seriesColor;
            sparklineGroup.LineWeight = 1.0;


            // Hämta den första sparkline att ta bort
            Sparkline sparklineToRemove = sparklineCollection[0];

            // Anropa Remove-metoden med sparkline-objektet
            sparklineCollection.Remove(sparklineToRemove);

            Console.WriteLine("Sparkline removed successfully");


            Console.WriteLine("after deleted---Sparkline count: " + sparklineCollection.Count);
            // Spara arbetsboken
            workbook.Save("SparklineRemoveDemo.xlsx");
        }
    }
}
```

### Se även

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



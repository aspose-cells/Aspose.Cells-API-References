---
title: "SparklineGroup.SparklineCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup egenskap. Hämtar samlingen av Sparkline-objekt"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/sparklinecollection/
---
## SparklineGroup.SparklineCollection property

Hämtar samlingen av [`Sparkline`](../../sparkline/) objekt.

```csharp
[Obsolete("Use SparklineGroup.Sparklines property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SparklineCollection SparklineCollection { get; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället SparklineGroup.Sparklines egenskap. Denna egenskap kommer att tas bort 12 månader senare sedan november 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupPropertySparklineCollectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för sparkline-diagram
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);
            worksheet.Cells["C1"].PutValue(15);
            worksheet.Cells["D1"].PutValue(30);

            try
            {
                // Definiera plats för sparklines
                CellArea location = new CellArea
                {
                    StartRow = 0,
                    EndRow = 0,
                    StartColumn = 4,
                    EndColumn = 4
                };

                // Lägg till en sparkline‑grupp i kalkylbladet
                int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, location);
                SparklineGroup sparklineGroup = worksheet.SparklineGroups[groupIndex];

                // Lägg till en sparkline i gruppen
                sparklineGroup.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

                // Åtkomst till SparklineCollection-egenskap (skrivskyddad)
                SparklineCollection sparklineCollection = sparklineGroup.SparklineCollection;

                // Visa information om sparkline-samlingen
                Console.WriteLine($"SparklineCollection contains {sparklineCollection.Count} sparklines");

                // Iterera genom sparklines i samlingen
                for (int i = 0; i < sparklineCollection.Count; i++)
                {
                    Sparkline sparkline = sparklineCollection[i];
                    Console.WriteLine($"Sparkline {i + 1} location: Row {sparkline.Row}, Column {sparkline.Column}");
                }

                // Spara arbetsboken
                workbook.Save("SparklineCollectionDemo.xlsx");
                Console.WriteLine("SparklineCollection demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



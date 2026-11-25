---
title: "SparklineGroup.SparklineCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Ottiene la raccolta di oggetti Sparkline"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/sparklinecollection/
---
## SparklineGroup.SparklineCollection property

Ottiene la raccolta di oggetto [`Sparkline`](../../sparkline/).

```csharp
[Obsolete("Use SparklineGroup.Sparklines property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SparklineCollection SparklineCollection { get; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà SparklineGroup.Sparklines. Questa proprietà sarà rimossa tra 12 mesi a partire da novembre 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per le sparklines
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);
            worksheet.Cells["C1"].PutValue(15);
            worksheet.Cells["D1"].PutValue(30);

            try
            {
                // Definisci la posizione per le sparklines
                CellArea location = new CellArea
                {
                    StartRow = 0,
                    EndRow = 0,
                    StartColumn = 4,
                    EndColumn = 4
                };

                // Aggiungi un gruppo di sparkline al foglio di lavoro
                int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, location);
                SparklineGroup sparklineGroup = worksheet.SparklineGroups[groupIndex];

                // Aggiungi uno sparkline al gruppo
                sparklineGroup.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

                // Accedi alla proprietà SparklineCollection (sola lettura)
                SparklineCollection sparklineCollection = sparklineGroup.SparklineCollection;

                // Visualizza le informazioni sulla raccolta di sparkline
                Console.WriteLine($"SparklineCollection contains {sparklineCollection.Count} sparklines");

                // Itera attraverso le sparklines nella raccolta
                for (int i = 0; i < sparklineCollection.Count; i++)
                {
                    Sparkline sparkline = sparklineCollection[i];
                    Console.WriteLine($"Sparkline {i + 1} location: Row {sparkline.Row}, Column {sparkline.Column}");
                }

                // Salva la cartella di lavoro
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

### Vedi anche

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



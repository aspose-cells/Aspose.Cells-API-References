---
title: "SparklineCollection.Remove"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "metodo SparklineCollection. Rimuove lo sparkline"
type: docs
url: /it/net/aspose.cells.charts/sparklinecollection/remove/
---
## SparklineCollection.Remove method

Rimuove lo sparkline

```csharp
[Obsolete("Use SparklineCollection.RemoveSparkline(Sparkline) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Remove(object o)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | Object |  |

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo RemoveSparkline(). Questo metodo sarà rimosso tra 6 mesi a partire da dicembre 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

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
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserisci dati di esempio nel foglio di lavoro
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);


            // Definisci il CellArea dove verranno aggiunti gli sparklines
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };

            // Aggiungi un nuovo SparklineGroup al foglio di lavoro
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];

            SparklineCollection sparklineCollection = sparklineGroup.Sparklines;

            // Aggiungi sparklines al SparklineGroup
            sparklineCollection.Add("A1:D1", 0, 5);

            Console.WriteLine("Sparkline count: " + sparklineCollection.Count);

            // Imposta varie proprietà per il SparklineGroup
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;

            // Imposta i colori per i punti alti e bassi
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = System.Drawing.Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = System.Drawing.Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Imposta il colore della serie e lo spessore della linea
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = System.Drawing.Color.Orange;
            sparklineGroup.SeriesColor = seriesColor;
            sparklineGroup.LineWeight = 1.0;


            // Ottieni il primo sparkline da rimuovere
            Sparkline sparklineToRemove = sparklineCollection[0];

            // Chiama il metodo Remove con l'oggetto sparkline
            sparklineCollection.Remove(sparklineToRemove);

            Console.WriteLine("Sparkline removed successfully");


            Console.WriteLine("after deleted---Sparkline count: " + sparklineCollection.Count);
            // Salva la cartella di lavoro
            workbook.Save("SparklineRemoveDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



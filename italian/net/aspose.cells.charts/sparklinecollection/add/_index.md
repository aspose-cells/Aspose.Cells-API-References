---
title: "SparklineCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "metodo SparklineCollection. Aggiungi uno sparkline"
type: docs
url: /it/net/aspose.cells.charts/sparklinecollection/add/
---
## SparklineCollection.Add method

Aggiungi uno sparkline.

```csharp
public int Add(string dataRange, int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataRange | String | Specifica il nuovo intervallo di dati dello sparkline. |
| riga | Int32 | L'indice di riga della posizione. |
| colonna | Int32 | L'indice di colonna della posizione. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            for (int i = 0; i < 12; i++)
            {
                worksheet.Cells[4, 3 + i].PutValue(i + 1);
            }

            // Crea un gruppo di sparkline
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Aggiungi uno sparkline con intervallo di dati e posizione
            int sparklineIndex = group.Sparklines.Add("D5:O5", 4, 15);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



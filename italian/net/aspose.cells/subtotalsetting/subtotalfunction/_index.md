---
title: "SubtotalSetting.SubtotalFunction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SubtotalSetting. La funzione di subtotale"
type: docs
url: /it/net/aspose.cells/subtotalsetting/subtotalfunction/
---
## SubtotalSetting.SubtotalFunction property

La funzione di subtotale.

```csharp
public ConsolidationFunction SubtotalFunction { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertySubtotalFunctionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group A" : "Group B");
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Crea l'impostazione di subtotale recuperandola dai dati esistenti
            CellArea area = CellArea.CreateCellArea("A1", "B10");
            SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
            
            // Configura il subtotale - queste proprietà sono di sola lettura nell'API reale
            // Quindi utilizzeremo direttamente il metodo Subtotal con i parametri
            int groupBy = 0; // Group by first column
            ConsolidationFunction function = ConsolidationFunction.Sum;
            int[] subtotalColumns = new int[] {1}; // Subtotal on second column
            
            // Applica i subtotali
            worksheet.Cells.Subtotal(area, groupBy, function, subtotalColumns);

            // Verifica la proprietà SubtotalFunction dall'impostazione recuperata
            Console.WriteLine("Subtotal Function: " + subtotalSetting.SubtotalFunction);
            
            // Salva la cartella di lavoro
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



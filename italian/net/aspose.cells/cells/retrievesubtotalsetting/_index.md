---
title: "Cells.RetrieveSubtotalSetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Recupera l'impostazione dei subtotali dell'intervallo"
type: docs
url: /it/net/aspose.cells/cells/retrievesubtotalsetting/
---
## Cells.RetrieveSubtotalSetting method

Recupera le impostazioni dei subtotali dell'intervallo.

```csharp
public SubtotalSetting RetrieveSubtotalSetting(CellArea ca)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | CellArea | L'intervallo |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRetrieveSubtotalSettingWithCellAreaDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per i subtotali
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group1" : "Group2");
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Crea subtotali
            CellArea area = CellArea.CreateCellArea("A1", "B10");
            worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 });

            // Recupera le impostazioni dei subtotali
            SubtotalSetting setting = worksheet.Cells.RetrieveSubtotalSetting(area);

            // Impostazioni di output
            Console.WriteLine("GroupBy: " + setting.GroupBy);
            Console.WriteLine("Function: " + setting.SubtotalFunction);
            Console.WriteLine("SummaryBelowData: " + setting.SummaryBelowData);
            Console.WriteLine("TotalList: " + string.Join(",", setting.TotalList));
        }
    }
}
```

### Vedi anche

* class [SubtotalSetting](../../subtotalsetting/)
* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



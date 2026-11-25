---
title: "SubtotalSetting.TotalList"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SubtotalSetting. Un array di offset di campo a base zero che indica i campi a cui vengono aggiunti i subtotali"
type: docs
url: /it/net/aspose.cells/subtotalsetting/totallist/
---
## SubtotalSetting.TotalList property

Un array di offset di campo basati su zero, che indica i campi a cui vengono aggiunti i subtotali.

```csharp
public int[] TotalList { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertyTotalListDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Configurazione dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Crea e applica il subtotale
            CellArea area = CellArea.CreateCellArea("A1", "B5");
            worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 }, true, true, true);

            // Recupera l'impostazione di subtotale per dimostrare l'uso di TotalList
            SubtotalSetting subtotal = worksheet.Cells.RetrieveSubtotalSetting(area);
            Console.WriteLine("TotalList contains column index: " + subtotal.TotalList[0]);
            
            // Salva la cartella di lavoro
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



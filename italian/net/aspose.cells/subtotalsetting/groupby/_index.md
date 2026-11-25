---
title: "SubtotalSetting.GroupBy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SubtotalSetting. Il campo su cui raggruppare come offset intero a base zero"
type: docs
url: /it/net/aspose.cells/subtotalsetting/groupby/
---
## SubtotalSetting.GroupBy property

Il campo per il raggruppamento, come offset intero a base zero

```csharp
public int GroupBy { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SubtotalSettingPropertyGroupByDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Group A");
            worksheet.Cells["A3"].PutValue("Group B");
            worksheet.Cells["A4"].PutValue("Group A");
            worksheet.Cells["A5"].PutValue("Group B");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["B5"].PutValue(400);

            try
            {
                // Definisci l'area della cella per i subtotali
                CellArea area = CellArea.CreateCellArea("A1", "B5");

                // Applica i subtotali ai dati
                worksheet.Cells.Subtotal(
                    area,
                    0, // Group by first column (Category)
                    ConsolidationFunction.Sum,
                    new int[] { 1 }, // Subtotal on second column (Value)
                    true,
                    true,
                    true);

                // Recupera l'impostazione di subtotale per accedere alla proprietà GroupBy
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // Visualizza il valore della proprietà GroupBy
                Console.WriteLine("GroupBy field index: " + subtotalSetting.GroupBy);

                // Salva la cartella di lavoro
                workbook.Save("GroupByDemo.xlsx");
                Console.WriteLine("Subtotal with GroupBy demonstrated successfully.");
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

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



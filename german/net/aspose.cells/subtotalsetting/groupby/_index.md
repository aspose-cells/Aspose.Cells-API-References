---
title: "SubtotalSetting.GroupBy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SubtotalSetting‑Eigenschaft. Das Feld, nach dem gruppiert wird, als nullbasierter ganzzahliger Offset"
type: docs
url: /de/net/aspose.cells/subtotalsetting/groupby/
---
## SubtotalSetting.GroupBy property

Das Feld, nach dem gruppiert wird, als nullbasierter ganzzahliger Offset.

```csharp
public int GroupBy { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SubtotalSettingPropertyGroupByDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
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
                // Definieren Sie den Zellbereich für Zwischensummen.
                CellArea area = CellArea.CreateCellArea("A1", "B5");

                // Wenden Sie Zwischensummen auf die Daten an.
                worksheet.Cells.Subtotal(
                    area,
                    0, // Group by first column (Category)
                    ConsolidationFunction.Sum,
                    new int[] { 1 }, // Subtotal on second column (Value)
                    true,
                    true,
                    true);

                // Rufen Sie die Zwischensummen‑Einstellung ab, um auf die GroupBy‑Eigenschaft zuzugreifen
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // Zeigen Sie den Wert der GroupBy‑Eigenschaft an
                Console.WriteLine("GroupBy field index: " + subtotalSetting.GroupBy);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



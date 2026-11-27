---
title: "SubtotalSetting.GroupBy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SubtotalSetting property. Fältet att gruppera efter som ett nollbaserat heltalsoffset"
type: docs
url: /sv/net/aspose.cells/subtotalsetting/groupby/
---
## SubtotalSetting.GroupBy property

Fältet att gruppera efter, som ett nollbaserat heltalsavstånd

```csharp
public int GroupBy { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SubtotalSettingPropertyGroupByDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
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
                // Definiera cellområdet för delsummeringar
                CellArea area = CellArea.CreateCellArea("A1", "B5");

                // Tillämpa delsummeringar på data
                worksheet.Cells.Subtotal(
                    area,
                    0, // Group by first column (Category)
                    ConsolidationFunction.Sum,
                    new int[] { 1 }, // Subtotal on second column (Value)
                    true,
                    true,
                    true);

                // Hämta subtotalinställningen för att komma åt GroupBy-egenskapen
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // Visa värdet för GroupBy-egenskapen
                Console.WriteLine("GroupBy field index: " + subtotalSetting.GroupBy);

                // Spara arbetsboken
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

### Se även

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



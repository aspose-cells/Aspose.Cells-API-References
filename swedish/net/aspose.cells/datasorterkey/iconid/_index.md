---
title: "DataSorterKey.IconId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorterKey-egenskap. Representerar id för ikonsättstypen"
type: docs
url: /sv/net/aspose.cells/datasorterkey/iconid/
---
## DataSorterKey.IconId property

Representerar id för ikonsättstypen.

```csharp
public int IconId { get; }
```

### Anmärkningar

Gäller endast när [`Type`](../type/) är Icon.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterKeyPropertyIconIdDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med värden som kan använda ikonsätt
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Lägg till villkorsformatering med ikonset
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = CellArea.CreateCellArea("A1", "A5");
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.IconSet);
            fcc[0].IconSet.Type = IconSetType.Arrows3;

            // Skapa datasortering och lägg till nyckel
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Sortera data
            sorter.Sort(worksheet.Cells, area);

            try
            {
                // Visa IconId-egenskapen från sorteringsnycklarna
                foreach (DataSorterKey key in sorter.Keys)
                {
                    Console.WriteLine($"IconId: {key.IconId}");
                    Console.WriteLine($"IconSetType: {key.IconSetType}");
                }

                // Spara arbetsboken
                workbook.Save("IconIdDemo.xlsx");
                Console.WriteLine("IconId demonstration completed successfully.");
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

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



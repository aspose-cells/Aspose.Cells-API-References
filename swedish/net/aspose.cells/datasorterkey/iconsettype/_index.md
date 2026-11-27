---
title: "DataSorterKey.IconSetType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorterKey‑egenskap. Representerar ikonsättstypen"
type: docs
url: /sv/net/aspose.cells/datasorterkey/iconsettype/
---
## DataSorterKey.IconSetType property

Representerar ikonsättstypen.

```csharp
public IconSetType IconSetType { get; }
```

### Anmärkningar

Gäller endast när [`Type`](../type/) är Icon.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // Skapa ett arbetsbok-objekt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med villkorsformatering för icon set
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

            // Skapa datasortering med ikonsättstyp
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Sortera data
            sorter.Sort(worksheet.Cells, area);

            // Visa ikonsättstypen från sorteringsnyckeln
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"IconSetType used for sorting: {key.IconSetType}");
            }

            // Spara arbetsboken
            workbook.Save("IconSetTypeSortingDemo.xlsx");
        }
    }
}
```

### Se även

* enum [IconSetType](../../iconsettype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



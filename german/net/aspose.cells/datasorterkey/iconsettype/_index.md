---
title: "DataSorterKey.IconSetType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorterKey-Eigenschaft. Stellt den Icon-Set-Typ dar"
type: docs
url: /de/net/aspose.cells/datasorterkey/iconsettype/
---
## DataSorterKey.IconSetType property

Stellt den Symbolsatztyp dar.

```csharp
public IconSetType IconSetType { get; }
```

### Hinweise

Wirkt nur, wenn [`Type`](../type/) Icon ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // Ein Arbeitsmappenobjekt erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten mit bedingter Formatierung des Icon-Sets hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Fügen Sie eine bedingte Formatierung für das Symbolset hinzu
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = CellArea.CreateCellArea("A1", "A5");
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.IconSet);
            fcc[0].IconSet.Type = IconSetType.Arrows3;

            // Erstellen Sie einen DataSorter mit Icon-Set-Typ
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Daten sortieren
            sorter.Sort(worksheet.Cells, area);

            // Zeigen Sie den Icon-Set-Typ des Sorter-Schlüssels an
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"IconSetType used for sorting: {key.IconSetType}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("IconSetTypeSortingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [IconSetType](../../iconsettype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



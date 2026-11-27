---
title: "Klass DataSorterKey"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DataSorterKey-klass. Representerar nyckeln för datasorteringen"
type: docs
url: /sv/net/aspose.cells/datasorterkey/
---
## DataSorterKey class

Representerar nyckeln för datasorteringen.

```csharp
public class DataSorterKey
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Color](../../aspose.cells/datasorterkey/color/) { get; } | Hämtar den sorterade färgen. |
| [IconId](../../aspose.cells/datasorterkey/iconid/) { get; } | Representerar id för ikonsättstypen. |
| [IconSetType](../../aspose.cells/datasorterkey/iconsettype/) { get; } | Representerar ikonsättstypen. |
| [Index](../../aspose.cells/datasorterkey/index/) { get; } | Hämtar det sorterade kolumnindexet (absolut position, kolumn A är 0, B är 1, ...). |
| [Order](../../aspose.cells/datasorterkey/order/) { get; } | Anger sorteringsordningen. |
| [Type](../../aspose.cells/datasorterkey/type/) { get; } | Representerar sorteringstypen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataSorterKeyDemo
    {
        public static void DataSorterKeyExample()
        {
            // Skapa ett arbetsbok-objekt och läs in en mallfil
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till några exempeldata att sortera
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Instansiera datasorteringsobjektet
            DataSorter sorter = workbook.DataSorter;

            // Lägg till nyckel för den första kolumnen (A) för att sortera i stigande ordning
            sorter.AddKey(0, SortOrder.Ascending);

            // Skapa ett cellområde (intervall) att sortera
            CellArea ca = CellArea.CreateCellArea("A1", "A5");

            // Utför sorteringen
            sorter.Sort(worksheet.Cells, ca);

            // Spara utdatafilen
            workbook.Save("DataSorterKeyExample.xlsx");
            workbook.Save("DataSorterKeyExample.pdf");

            // Få åtkomst till DataSorterKeyCollection
            DataSorterKeyCollection keys = sorter.Keys;

            // Iterera genom nycklarna och skriv ut deras egenskaper
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Order: {key.Order}");
                Console.WriteLine($"Index: {key.Index}");
                Console.WriteLine($"Type: {key.Type}");
                Console.WriteLine($"IconSetType: {key.IconSetType}");
                Console.WriteLine($"IconId: {key.IconId}");
                Console.WriteLine($"Color: {key.Color}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



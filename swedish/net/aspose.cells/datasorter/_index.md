---
title: "Klass DataSorter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DataSorter klass. Sammanfattande beskrivning för DataSorter"
type: docs
url: /sv/net/aspose.cells/datasorter/
---
## DataSorter class

Sammanfattande beskrivning för DataSorter.

```csharp
public class DataSorter
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CaseSensitive](../../aspose.cells/datasorter/casesensitive/) { get; set; } | Hämtar och anger om skiftlägeskänslighet vid jämförelse av sträng. |
| [HasHeaders](../../aspose.cells/datasorter/hasheaders/) { get; set; } | Representerar om intervallet har rubriker. |
| [Key1](../../aspose.cells/datasorter/key1/) { get; set; } | Representerar första sorterade kolumnens index (absolut position, kolumn A är 0, B är 1, ...). |
| [Key2](../../aspose.cells/datasorter/key2/) { get; set; } | Representerar andra sorterade kolumnens index (absolut position, kolumn A är 0, B är 1, ...). |
| [Key3](../../aspose.cells/datasorter/key3/) { get; set; } | Representerar tredje sorterade kolumnens index (absolut position, kolumn A är 0, B är 1, ...). |
| [Keys](../../aspose.cells/datasorter/keys/) { get; } | Hämtar nyckellistan för data sorter. |
| [Order1](../../aspose.cells/datasorter/order1/) { get; set; } | Representerar sorteringsordning för den första nyckeln. |
| [Order2](../../aspose.cells/datasorter/order2/) { get; set; } | Representerar sorteringsordning för den andra nyckeln. |
| [Order3](../../aspose.cells/datasorter/order3/) { get; set; } | Representerar sorteringsordning för den tredje nyckeln. |
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber/) { get; set; } | Indikerar om sortering av allt som ser ut som ett tal. |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright/) { get; set; } | Sant betyder att sorteringsriktningen är från vänster till höger. Falskt betyder att sorteringsriktningen är från topp till botten. Standardvärdet är falskt. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddColorKey](../../aspose.cells/datasorter/addcolorkey/)(int, SortOnType, SortOrder, Color) | Lägger till färgsorteringsnyckel. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_1)(int, SortOrder) | Lägger till sorterat kolumnindex och sorteringsordning. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_2)(int, SortOrder, string) | Lägger till sorterat kolumnindex och sorteringsordning med anpassad sorteringslista. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_3)(int, SortOrder, string[]) | Lägger till sorterat kolumnindex och sorteringsordning med anpassad sorteringslista. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey)(int, SortOnType, SortOrder, object) | Lägger till sorterat kolumnindex och sorteringsordning med anpassad sorteringslista. |
| [Clear](../../aspose.cells/datasorter/clear/)() | Rensa alla inställningar. |
| [Sort](../../aspose.cells/datasorter/sort/#sort)() | Sortera data i intervallet. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_1)(Cells, CellArea) | Sortera data i området. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_2)(Cells, int, int, int, int) | Sorterar data i området. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterDemo
    {
        public static void DataSorterExample()
        {
            // Instansiera ett nytt Workbook-objekt
            Workbook workbook = new Workbook("DataSorter_original.xlsx");

            // Hämta workbook DataSorter-objektet
            DataSorter sorter = workbook.DataSorter;

            // Ställ in den första ordningen för DataSorter-objektet
            sorter.Order1 = SortOrder.Descending;
            // Definiera den första nyckeln
            sorter.Key1 = 0;

            // Ställ in den andra ordningen för DataSorter-objektet
            sorter.Order2 = SortOrder.Ascending;
            // Definiera den andra nyckeln
            sorter.Key2 = 1;

            // Skapa ett cellområde (intervall)
            CellArea ca = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 13,
                EndColumn = 1
            };

            // Sortera data i det angivna dataområdet (A1:B14)
            sorter.Sort(workbook.Worksheets[0].Cells, ca);

            // Spara Excel-filen
            workbook.Save("DataSorterExample.xlsx");
            workbook.Save("DataSorterExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



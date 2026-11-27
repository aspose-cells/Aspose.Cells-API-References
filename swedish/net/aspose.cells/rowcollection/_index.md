---
title: "Klass RowCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.RowCollection-klass. Samlar Row-objekten som representerar de enskilda raderna i ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/rowcollection/
---
## RowCollection class

Samlar [`Row`](../row/) objekten som representerar de enskilda raderna i ett kalkylblad.

```csharp
public class RowCollection : IEnumerable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Count](../../aspose.cells/rowcollection/count/) { get; } | Hämtar antalet rader i denna samling. |
| [Item](../../aspose.cells/rowcollection/item/) { get; } | Hämtar ett [`Row`](../row/) objekt med angivet radindex. Row-objektet för det angivna radindexet kommer att instansieras om det inte redan finns. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Clear](../../aspose.cells/rowcollection/clear/)() | Rensa alla rader och celler. |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator)() | Hämtar en enumerator som itererar rader genom denna samling |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator_1)(bool, bool) | Hämtar en enumerator som itererar rader genom denna samling |
| [GetRowByIndex](../../aspose.cells/rowcollection/getrowbyindex/)(int) | Hämtar radobjektet efter positionen i listan. |
| [RemoveAt](../../aspose.cells/rowcollection/removeat/)(int) | Ta bort radobjektet på det angivna indexet (positionen) i denna samling. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionDemo
    {
        public static void RowCollectionExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Hämtning av referensen till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("Aspose.Cells");
            // Hämta Rows-samlingen
            RowCollection rows = worksheet.Cells.Rows;

            // Hämta antalet rader i samlingen
            int rowCount = rows.Count;
            Console.WriteLine("Number of rows: " + rowCount);

            // Hämta den första raden
            Row firstRow = rows[0];
            Console.WriteLine("First row index: " + firstRow.Index);

            // Iterera genom raderna med GetEnumerator
            IEnumerator enumerator = rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine("Row index: " + row.Index + ", Height: " + row.Height);
            }

            // Hämta en rad med index
            Row specificRow = rows.GetRowByIndex(1);
            Console.WriteLine("Specific row index: " + specificRow.Index);

            // Rensa alla rader och celler
            rows.Clear();
            Console.WriteLine("Rows cleared.");

            // Spara arbetsboken
            workbook.Save("RowCollectionExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



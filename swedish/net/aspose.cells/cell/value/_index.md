---
title: "Cell.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cellegenskap. Hämtar/sätter värdet som finns i den här cellen"
type: docs
url: /sv/net/aspose.cells/cell/value/
---
## Cell.Value property

Hämtar/anger värdet som finns i den här cellen.

```csharp
public object Value { get; set; }
```

### Anmärkningar

Möjlig typ:

null,

Boolean,

DateTime,

Double,

Integer

String.

För heltalsvärden kan de returneras som ett Integer‑objekt eller ett Double‑objekt. Det finns ingen garanti för att det returnerade värdet alltid behålls som samma objekttyp.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange värden med Value‑egenskapen
            cells[0, 0].Value = "Product ID";
            cells[0, 1].Value = "Product Name";
            
            // Visa exempel på null‑värden
            cells[0, 2].Value = null;
            cells[1, 0].Value = null;
            cells[1, 1].Value = null;
            cells[1, 2].Value = null;

            // Visa värden
            Console.WriteLine("Cell[0,0] Value: " + cells[0, 0].Value);
            Console.WriteLine("Cell[0,1] Value: " + cells[0, 1].Value);
            Console.WriteLine("Cell[0,2] Value: " + (cells[0, 2].Value == null ? "null" : cells[0, 2].Value));
            Console.WriteLine("Cell[1,0] Value: " + (cells[1, 0].Value == null ? "null" : cells[1, 0].Value));
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Cell.SharedStyleIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑egenskap. Hämtar cellens delade stilindex i stilpoolen"
type: docs
url: /sv/net/aspose.cells/cell/sharedstyleindex/
---
## Cell.SharedStyleIndex property

Hämtar cellens delade stilindex i stilpoolen.

```csharp
public int SharedStyleIndex { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertySharedStyleIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en stil och ange några egenskaper
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;

            // Applicera stilen på cell A1
            worksheet.Cells["A1"].SetStyle(style);

            // Hämta den delade stilindexen för cell A1
            int sharedStyleIndex = worksheet.Cells["A1"].SharedStyleIndex;

            // Hämta stilen från stilpoolen med hjälp av indexet
            Style retrievedStyle = workbook.GetStyleInPool(sharedStyleIndex);

            // Skriv ut stilinformation för att verifiera
            Console.WriteLine("Font Name: " + retrievedStyle.Font.Name);
            Console.WriteLine("Font Size: " + retrievedStyle.Font.Size);
            Console.WriteLine("Is Bold: " + retrievedStyle.Font.IsBold);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "FindOptions.LookInType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FindOptions-egenskap. Typ att söka i"
type: docs
url: /sv/net/aspose.cells/findoptions/lookintype/
---
## FindOptions.LookInType property

Titta i typen.

```csharp
public LookInType LookInType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookInTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och lägg till exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange värden och formler i celler
            worksheet.Cells["A1"].PutValue("SearchValue");
            worksheet.Cells["A2"].Formula = "=A1";
            worksheet.Cells["B1"].PutValue("OtherValue");

            // Skapa sökalternativ för att endast söka i formler
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            // Sök efter värdet i formler
            Cell foundCell = worksheet.Cells.Find("SearchValue", null, options);

            // Skriv ut resultatet
            if (foundCell != null)
            {
                Console.WriteLine($"Found at: Row {foundCell.Row}, Column {foundCell.Column}");
            }
            else
            {
                Console.WriteLine("Value not found in formulas");
            }
        }
    }
}
```

### Se även

* enum [LookInType](../../lookintype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



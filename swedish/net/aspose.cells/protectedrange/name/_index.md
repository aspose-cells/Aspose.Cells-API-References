---
title: "ProtectedRange.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ProtectedRange-egenskap. Hämtar områdestiteln. Detta används som en beskrivning, inte som en namngiven områdesdefinition"
type: docs
url: /sv/net/aspose.cells/protectedrange/name/
---
## ProtectedRange.Name property

Hämtar områdestiteln. Den används som en beskrivning, inte som en namngiven områdesdefinition.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa samling av skyddade områden
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // Lägg till ett skyddat område med namnet "MyRange"
            int index = allowRanges.Add("MyRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];
            protectedRange.Password = "123";

            // Åtkomst och visa Name-egenskapen
            Console.WriteLine("Protected range name: " + protectedRange.Name);
            Console.WriteLine("Cell area: {0},{1} to {2},{3}", 
                protectedRange.CellArea.StartRow,
                protectedRange.CellArea.StartColumn,
                protectedRange.CellArea.EndRow,
                protectedRange.CellArea.EndColumn);

            // Lägg till ett annat namngivet område
            index = allowRanges.Add("SecondRange", 3, 3, 5, 5);
            ProtectedRange secondRange = allowRanges[index];
            Console.WriteLine("Second protected range name: " + secondRange.Name);

            // Spara arbetsboken
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



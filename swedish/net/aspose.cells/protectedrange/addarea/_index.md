---
title: "ProtectedRange.AddArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ProtectedRange-metod. Lägger till ett refererat område till detta"
type: docs
url: /sv/net/aspose.cells/protectedrange/addarea/
---
## ProtectedRange.AddArea method

Lägger till ett refererat område till detta

```csharp
public void AddArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startraden. |
| startColumn | Int32 | Startkolumnen. |
| endRow | Int32 | Slutrad. |
| endColumn | Int32 | Slutkolumn. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectedRangeMethodAddAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add returnerar index för den nya ProtectedRange i samlingen
            int protectedRangeIndex = worksheet.AllowEditRanges.Add("DemoProtectedRange", 0, 0, 0, 0);
            ProtectedRange protectedRange = worksheet.AllowEditRanges[protectedRangeIndex];

            try
            {
                protectedRange.AddArea(2, 2, 5, 5);
                Console.WriteLine("Added new area to protected range.");

                CellArea[] areas = protectedRange.GetAreas();
                Console.WriteLine($"Total protected areas: {areas.Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            worksheet.Protect(ProtectionType.All, "password123", null);
            workbook.Save("ProtectedRangeAddAreaDemo.xlsx");
        }
    }
}
```

### Se även

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



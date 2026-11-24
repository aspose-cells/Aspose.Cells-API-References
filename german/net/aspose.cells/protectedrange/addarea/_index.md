---
title: "ProtectedRange.AddArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ProtectedRange-Methode. Fügt diesem einen referenzierten Bereich hinzu"
type: docs
url: /de/net/aspose.cells/protectedrange/addarea/
---
## ProtectedRange.AddArea method

Fügt diesem einen referenzierten Bereich hinzu.

```csharp
public void AddArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Startzeile. |
| startColumn | Int32 | Die Startspalte. |
| endRow | Int32 | Die Endzeile. |
| endColumn | Int32 | Die Endspalte. |

### Beispiele

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

            // Add gibt den Index des neuen ProtectedRange in der Sammlung zurück
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

### Siehe auch

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



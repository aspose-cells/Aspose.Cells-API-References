---
title: "ProtectedRange.AddArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ProtectedRange yöntemi. Bu nesneye başvurulan bir alan ekler"
type: docs
url: /tr/net/aspose.cells/protectedrange/addarea/
---
## ProtectedRange.AddArea method

Bu öğeye bir başvurulan alan ekler.

```csharp
public void AddArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Başlangıç satırı. |
| startColumn | Int32 | Başlangıç sütunu. |
| endRow | Int32 | Bitiş satırı. |
| endColumn | Int32 | Bitiş sütunu. |

### Örnekler

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

            // Add, koleksiyondaki yeni ProtectedRange'in dizinini döndürür
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

### Ayrıca Bakınız

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



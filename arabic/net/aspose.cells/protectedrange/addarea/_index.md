---
title: "ProtectedRange.AddArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ProtectedRange. تضيف منطقة مُشار إليها إلى هذا"
type: docs
url: /ar/net/aspose.cells/protectedrange/addarea/
---
## ProtectedRange.AddArea method

يضيف مساحة مُشار إليها إلى هذا

```csharp
public void AddArea(int startRow, int startColumn, int endRow, int endColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | صف البداية. |
| startColumn | Int32 | عمود البداية. |
| endRow | Int32 | صف النهاية. |
| endColumn | Int32 | عمود النهاية. |

### أمثلة

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

            // إضافة تُعيد فهرس ProtectedRange الجديد في المجموعة
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

### انظر أيضًا

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



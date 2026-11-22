---
title: "تعداد LookAtType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.LookAtType. يمثل نوع LookAt"
type: docs
url: /ar/net/aspose.cells/lookattype/
---
## LookAtType enumeration

يمثل نوع النظرة إلى.

```csharp
public enum LookAtType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Contains | `0` | قيمة الخلية تحتوي على كائن البحث. |
| StartWith | `1` | قيمة الخلية تبدأ بكائن البحث. |
| EndWith | `2` | قيمة الخلية تنتهي بكائن البحث. |
| EntireContent | `3` | قيمة الخلية هي نفسها كائن البحث. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LookAtTypeDemo
    {
        public static void LookAtTypeExample()
        {
            // إنشاء كائن دفتر العمل
            Workbook workbook = new Workbook("LookAtTypeExample_original.xlsx");

            // الحصول على مجموعة Cells
            Cells cells = workbook.Worksheets[0].Cells;

            // إنشاء كائن FindOptions
            FindOptions findOptions = new FindOptions();

            // إنشاء منطقة Cells
            CellArea ca = new CellArea();
            ca.StartRow = 8;
            ca.StartColumn = 2;
            ca.EndRow = 17;
            ca.EndColumn = 13;

            // تعيين منطقة الخلايا لFindOptions
            findOptions.SetRange(ca);

            // تعيين خصائص البحث
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // تعيين LookAtType إلى Contains
            findOptions.LookAtType = LookAtType.Contains;

            // ابحث عن الخلية ذات قيمة محددة
            Cell cell = cells.Find("searchValue", null, findOptions);

            if (cell != null)
            {
                Console.WriteLine($"Cell found at row {cell.Row}, column {cell.Column}");
            }
            else
            {
                Console.WriteLine("Cell not found.");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



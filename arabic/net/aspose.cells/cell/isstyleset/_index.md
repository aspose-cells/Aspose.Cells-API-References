---
title: "Cell.IsStyleSet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تشير إلى ما إذا تم تعيين نمط الخلية. إذا كان الإرجاع false فهذا يعني أن هذه الخلية لها تنسيق خلية افتراضي"
type: docs
url: /ar/net/aspose.cells/cell/isstyleset/
---
## Cell.IsStyleSet property

يشير إلى ما إذا تم تعيين نمط الخلية. إذا تم إرجاع false، فهذا يعني أن هذه الخلية لديها تنسيق خلية افتراضي.

```csharp
public bool IsStyleSet { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsStyleSetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // الوصول إلى خلية لم يتم تنسيقها بعد
            Cell unsetStyleCell = cells["A1"];
            Console.WriteLine($"Cell A1 IsStyleSet before styling: {unsetStyleCell.IsStyleSet}");

            // قم بتنسيق خلية مختلفة
            Cell styledCell = cells["B2"];
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            styledCell.SetStyle(style);

            Console.WriteLine($"Cell B2 IsStyleSet after styling: {styledCell.IsStyleSet}");

            // تحقق مما إذا كان النمط موروثًا من الصف
            Row row = cells.Rows[4];
            row.SetStyle(style);
            Cell rowInheritedCell = cells["E4"];
            Console.WriteLine($"Cell E4 IsStyleSet (inherited from row): {rowInheritedCell.IsStyleSet}");

            // تعيين النمط صراحةً إلى null لخلية
            Cell nullStyleCell = cells["C3"];
            nullStyleCell.SetStyle(null);
            Console.WriteLine($"Cell C3 IsStyleSet after setting null: {nullStyleCell.IsStyleSet}");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Worksheet.UnFreezePanes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. يزيل تجميد الألواح في ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/unfreezepanes/
---
## Worksheet.UnFreezePanes method

يفك تجميد الألواح في ورقة العمل.

```csharp
public void UnFreezePanes()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnFreezePanesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // تجميد الألواح عند الخلية C3 (الصفوف 2، الأعمدة 2 مجمّدة)
            worksheet.FreezePanes("C3", 2, 2);

            // تحقق من تجميد الألواح
            int frozenRow, frozenColumn, frozenRows, frozenColumns;
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"Frozen panes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // إلغاء تجميد الألواح
            worksheet.UnFreezePanes();

            // تحقق من إلغاء تجميد الألواح
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"After UnFreezePanes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // احفظ المصنف
            workbook.Save("UnFreezePanesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



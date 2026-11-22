---
title: "Worksheet.IsRowColumnHeadersVisible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل أو تعيّن قيمة تشير إلى ما إذا كانت ورقة العمل ستعرض رؤوس الصفوف والأعمدة. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/worksheet/isrowcolumnheadersvisible/
---
## Worksheet.IsRowColumnHeadersVisible property

يحصل على أو يضبط قيمة تشير إلى ما إذا كانت ورقة العمل ستعرض رؤوس الصفوف والأعمدة. القيمة الافتراضية هي true.

```csharp
public bool IsRowColumnHeadersVisible { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRowColumnHeadersVisibleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين رؤية رؤوس الصفوف والأعمدة إلى false
            worksheet.IsRowColumnHeadersVisible = false;
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // حمّل دفتر العمل المحفوظ للتحقق من الخاصية
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // إخراج قيمة الخاصية
            Console.WriteLine("Row and Column Headers Visible: " + loadedWorksheet.IsRowColumnHeadersVisible);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



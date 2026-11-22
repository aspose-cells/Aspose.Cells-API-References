---
title: "Worksheet.GetPanes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تحصل على أجزاء النافذة"
type: docs
url: /ar/net/aspose.cells/worksheet/getpanes/
---
## Worksheet.GetPanes method

يحصل على ألواح النافذة.

```csharp
public PaneCollection GetPanes()
```

### ملاحظات

إذا لم تكن النافذة مقسمة أو مجمدة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetPanesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تجميد الأجزاء عند الصف 5 والعمود 3
            worksheet.FreezePanes(5, 3, 5, 3);
            
            // الحصول على معلومات الجزء
            PaneCollection panes = worksheet.GetPanes();
            
            // عرض معلومات الجزء
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            Console.WriteLine("First visible column of right pane: " + panes.FirstVisibleColumnOfRightPane);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PaneCollection](../../panecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



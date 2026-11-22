---
title: "Workbook.RemoveUnusedStyles"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. إزالة جميع الأنماط غير المستخدمة"
type: docs
url: /ar/net/aspose.cells/workbook/removeunusedstyles/
---
## Workbook.RemoveUnusedStyles method

إزالة جميع الأنماط غير المستخدمة.

```csharp
public void RemoveUnusedStyles()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveUnusedStylesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = wb.Worksheets[0];
            
            // إضافة بعض البيانات النموذجية مع الأنماط
            for (int i = 0; i < 10; i++)
            {
                Cell cell = sheet.Cells[i, 0];
                cell.PutValue("Item " + (i + 1));
                
                // تطبيق أنماط مختلفة على الخلايا
                Style style = wb.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 10 + i;
                style.Font.IsBold = i % 2 == 0;
                cell.SetStyle(style);
            }
            
            // إزالة بعض الخلايا لترك الأنماط غير المستخدمة
            sheet.Cells.DeleteRows(5, 5);
            
            // احفظ قبل إزالة الأنماط غير المستخدمة
            wb.Save("BeforeRemoveUnusedStyles.xlsx");
            
            // إزالة الأنماط غير المستخدمة
            wb.RemoveUnusedStyles();
            
            // حفظ بعد إزالة الأنماط غير المستخدمة
            wb.Save("AfterRemoveUnusedStyles.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



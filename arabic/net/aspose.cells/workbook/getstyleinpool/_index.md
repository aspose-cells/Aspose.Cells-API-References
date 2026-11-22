---
title: "Workbook.GetStyleInPool"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تحصل على النمط في مجموعة الأنماط. سيتم جمع جميع الأنماط في المصنف في مجموعة. هناك فهرس إشارة بسيط فقط في الخلايا"
type: docs
url: /ar/net/aspose.cells/workbook/getstyleinpool/
---
## Workbook.GetStyleInPool method

يحصل على النمط في مجموعة الأنماط. سيتم جمع جميع الأنماط في المصنف في مجموعة. هناك فهرس إشارة بسيط فقط في الخلايا.

```csharp
public Style GetStyleInPool(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | الفهرس. |

### قيمة الإرجاع

النمط في المجموعة يتطابق مع الفهرس المعطى، قد يكون فارغًا.

### ملاحظات

إذا تم تعديل النمط المرتجع، سيتغير نمط جميع الخلايا (التي تشير إلى هذا النمط).

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetStyleInPoolWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وإضافة بعض البيانات النموذجية
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123.45);
            ws.Cells["A3"].PutValue(DateTime.Now);
            
            // تطبيق بعض الأنماط
            Style style1 = wb.CreateStyle();
            style1.Custom = "$#,##0.00";
            ws.Cells["A2"].SetStyle(style1);
            
            Style style2 = wb.CreateStyle();
            style2.Custom = "yyyy-mm-dd";
            ws.Cells["A3"].SetStyle(style2);
            
            // حفظ إلى تدفق الذاكرة
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                
                // إعادة تحميل المصنف من التدفق
                ms.Position = 0;
                Workbook reloadWb = new Workbook(ms);
                
                // احصل على الأنماط وعرضها من مجموعة الأنماط
                int count = reloadWb.CountOfStylesInPool;
                Console.WriteLine($"Styles in pool: {count}");
                
                for (int i = 0; i < count; i++)
                {
                    Style style = reloadWb.GetStyleInPool(i);
                    Console.WriteLine($"Style {i}: CustomFormat={style.Custom}");
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



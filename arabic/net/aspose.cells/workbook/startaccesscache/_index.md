---
title: "Workbook.StartAccessCache"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تبدأ الجلسة التي تستخدم الذاكرات المؤقتة للوصول إلى البيانات"
type: docs
url: /ar/net/aspose.cells/workbook/startaccesscache/
---
## Workbook.StartAccessCache method

يبدأ الجلسة التي تستخدم الذاكرة المؤقتة للوصول إلى البيانات.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| opts | AccessCacheOptions | خيارات الوصول إلى البيانات |

### ملاحظات

إذا كان ذاكرة التخزين المؤقت للوصول إلى البيانات المحددة تتطلب أن تكون بعض نماذج البيانات في ورقة العمل "للقراءة فقط"، فسيتم اعتبار نماذج البيانات المقابلة في كل ورقة عمل في هذا الـWorkbook كـ"للقراءة فقط" ولا ينبغي للمستخدم تعديل أي منها. بعد الانتهاء من الوصول إلى البيانات، يجب استدعاء [`CloseAccessCache`](../closeaccesscache/) بنفس الخيارات لمسح جميع الذاكرات المؤقتة واستعادة وضع الوصول العادي.

### أمثلة

```csharp
using System;
using System.Drawing;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodStartAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // إضافة تنسيق شرطي
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            int index = cfc.Add();
            cfc[index].Add(CellArea.CreateCellArea(0, 0, 5, 0),
                FormatConditionType.DuplicateValues, OperatorType.None, null, null);
            
            // تعيين النمط للتنسيق الشرطي
            Style style = cfc[0][0].Style;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            
            // إضافة بعض الصور المضمنة
            Cells cells = sheet.Cells;
            byte[] img1 = File.ReadAllBytes("1.png");
            byte[] img2 = File.ReadAllBytes("2.png");
            cells[0, 0].EmbeddedImage = img1;
            cells[2, 0].EmbeddedImage = img2;
            cells[4, 0].EmbeddedImage = img1;

            // ابدأ ذاكرة الوصول المؤقت لتحسين الأداء
            wb.StartAccessCache(AccessCacheOptions.All);
            
            // الوصول إلى أنماط الخلايا (سيكون أسرع بفضل التخزين المؤقت)
            Console.WriteLine("A1 Pattern: " + cells[0, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A3 Pattern: " + cells[2, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A5 Pattern: " + cells[4, 0].GetDisplayStyle().Pattern);
            
            // إغلاق الذاكرة المؤقتة عند الانتهاء
            wb.CloseAccessCache(AccessCacheOptions.All);
        }
    }
}
```

### انظر أيضًا

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Worksheet.Workbook"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل على كائن المصنف الذي يحتوي على هذه الورقة"
type: docs
url: /ar/net/aspose.cells/worksheet/workbook/
---
## Worksheet.Workbook property

يحصل على كائن المصنف الذي يحتوي على هذه الورقة.

```csharp
public Workbook Workbook { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyWorkbookDemo
    {
        public static void Run()
        {
            // إنشاء مصنف مصدر والحصول على ورقة عمل
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // إضافة بيانات عينة إلى ورقة العمل المصدر
            sourceSheet.Cells["A1"].PutValue("Sample Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            
            // إنشاء دفتر عمل هدف
            Workbook destWorkbook = new Workbook();
            
            // نسخ السمة من مصنف المصدر باستخدام خاصية Worksheet.Workbook
            destWorkbook.CopyTheme(sourceSheet.Workbook);
            
            // الوصول إلى ورقة العمل الوجهة ونسخ البيانات
            Worksheet destSheet = destWorkbook.Worksheets[0];
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.CreateRange("A1:A3");
            Aspose.Cells.Range destRange = destSheet.Cells.CreateRange("A1:A3");
            
            // نسخ البيانات مع التنسيق
            destRange.Copy(sourceRange);
            
            // حفظ دفتر العمل الوجهة
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../../workbook/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



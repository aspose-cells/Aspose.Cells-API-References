---
title: "Style.Copy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Style. تنسخ البيانات من كائن نمط آخر"
type: docs
url: /ar/net/aspose.cells/style/copy/
---
## Style.Copy method

ينسخ البيانات من كائن نمط آخر

```csharp
public void Copy(Style style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | النمط | كائن Style المصدر |

### ملاحظات

هذه الطريقة لا تنسخ اسم النمط. إذا كنت تريد نسخ الاسم، يرجى استدعاء الشيفرات التالية بعد نسخ النمط: destStyle.Name = style.Name.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCopyWithStyleDemo
    {
        public static void Run()
        {
            // إنشاء مصنف المصدر مع بيانات عينة
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Sample Text");
            Style srcStyle = srcWorkbook.CreateStyle();
            srcStyle.Font.Name = "Arial";
            srcStyle.Font.Size = 14;
            srcSheet.Cells["A1"].SetStyle(srcStyle);

            // إنشاء دفتر عمل هدف
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // نسخ النمط من المصدر إلى الوجهة
            Style destStyle = destWorkbook.CreateStyle();
            destStyle.Copy(srcStyle);
            
            // تطبيق النمط المنسوخ
            destSheet.Cells["B2"].PutValue("Copied Style Text");
            destSheet.Cells["B2"].SetStyle(destStyle);

            // حفظ النتيجة
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



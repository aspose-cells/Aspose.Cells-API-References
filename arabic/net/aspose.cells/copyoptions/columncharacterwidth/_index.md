---
title: "CopyOptions.ColumnCharacterWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CopyOptions. تشير إلى ما إذا كان يتم نسخ عرض العمود بوحدة الأحرف"
type: docs
url: /ar/net/aspose.cells/copyoptions/columncharacterwidth/
---
## CopyOptions.ColumnCharacterWidth property

يشير إلى ما إذا كان يتم نسخ عرض العمود بوحدة الأحرف.

```csharp
public bool ColumnCharacterWidth { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyColumnCharacterWidthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل مصدر يحتوي على بيانات نموذجية
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // تعيين عرض العمود بالأحرف للتوضيح
            srcSheet.Cells.SetColumnWidth(0, 20); // 20 characters wide
            
            // أضف بعض البيانات التجريبية
            srcSheet.Cells["A1"].PutValue("Sample Text");
            srcSheet.Cells["A2"].PutValue("Another Sample");
            
            // إنشاء دفتر عمل هدف
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // نسخ مع تعيين ColumnCharacterWidth إلى true
            destSheet.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = true
            });
            
            // حفظ النتيجة
            destWorkbook.Save("output_with_column_width.xlsx", SaveFormat.Xlsx);
            
            // للمقارنة، نسخ بدون ColumnCharacterWidth
            Workbook destWorkbook2 = new Workbook();
            Worksheet destSheet2 = destWorkbook2.Worksheets[0];
            
            destSheet2.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = false
            });
            
            destWorkbook2.Save("output_without_column_width.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



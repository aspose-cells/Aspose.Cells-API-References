---
title: "StyleFlag.NumberFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعداد تنسيق الرقم"
type: docs
url: /ar/net/aspose.cells/styleflag/numberformat/
---
## StyleFlag.NumberFormat property

سيتم تطبيق إعداد تنسيق الأرقام.

```csharp
public bool NumberFormat { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyNumberFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // تعيين قيمة الخلية
            sheet.Cells[0, 0].Value = 1234.56;
            
            // إنشاء نمط تنسيق رقم مخصص
            Style style = workbook.CreateStyle();
            style.Custom = "_-€ #,##0.00;[Red]_-€ -#,##0.00";
            
            // تطبيق تنسيق الرقم فقط باستخدام StyleFlag
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            
            // تطبيق النمط على نطاق الخلايا (تحديد نوع Range بالكامل)
            Aspose.Cells.Range range = sheet.Cells.CreateRange(0, 0, 1, 1);
            range.ApplyStyle(style, styleFlag);
            
            // حفظ والتحقق
            workbook.Save("output_number_format.ods");
            
            // أعد التحميل للتحقق
            Workbook verifyWorkbook = new Workbook("output_number_format.ods");
            Worksheet verifySheet = verifyWorkbook.Worksheets[0];
            Console.WriteLine("Applied Number Format: " + verifySheet.Cells["A1"].GetStyle().Custom);
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



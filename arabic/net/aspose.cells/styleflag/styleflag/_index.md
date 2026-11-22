---
title: "StyleFlag.StyleFlag"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ StyleFlag. ينشئ كائنًا بجميع العلامات غير مفعلة"
type: docs
url: /ar/net/aspose.cells/styleflag/styleflag/
---
## StyleFlag constructor

ينشئ كائنًا بجميع العلامات مضبوطة على false.

```csharp
public StyleFlag()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نمط عريض
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // تطبيق النمط على الصف 9 باستخدام منشئ StyleFlag
            worksheet.Cells.ApplyRowStyle(9, boldStyle, new StyleFlag { FontBold = true });

            // إدخال قيمة في الخلية والتحقق من النمط
            worksheet.Cells[9, 0].PutValue("Bold Text");

            // احفظ المصنف
            workbook.Save("output.xlsx");

            Console.WriteLine("Style applied successfully using StyleFlag constructor.");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



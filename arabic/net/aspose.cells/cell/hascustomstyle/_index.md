---
title: "Cell.HasCustomStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تشير إلى ما إذا كانت هذه الخلية لديها إعدادات نمط مخصص تختلف عن النمط الافتراضي الموروث من الصف أو العمود أو المصنف المقابل"
type: docs
url: /ar/net/aspose.cells/cell/hascustomstyle/
---
## Cell.HasCustomStyle property

يشير إلى ما إذا كانت هذه الخلية لديها إعدادات نمط مخصصة (مختلفة عن الإعداد الافتراضي الموروث من الصف أو العمود أو دفتر العمل المقابل).

```csharp
public bool HasCustomStyle { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Check HasCustomStyle");

            // اعرض القيمة الأولية لخاصية HasCustomState (تورث النمط الافتراضي)
            Console.WriteLine("Initial HasCustomStyle: " + cell.HasCustomStyle);

            // أنشئ نمطًا مخصصًا وطبقه على الخلية
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.IsBold = true;
            cell.SetStyle(customStyle);

            // تحقق من أن HasCustomStyle true بعد تعديل النمط
            Console.WriteLine("After applying custom style - HasCustomStyle: " + cell.HasCustomStyle);

            // احفظ المصنف مع تطبيق النمط المخصص
            workbook.Save("CellCustomStyleDemo.xlsx");

            // أعد ضبط نمط الخلية إلى النمط الافتراضي للمصنف
            Style defaultStyle = workbook.DefaultStyle;
            cell.SetStyle(defaultStyle);

            // تحقق من أن HasCustomStyle false بعد العودة إلى الافتراضي
            Console.WriteLine("After resetting to default style - HasCustomStyle: " + cell.HasCustomStyle);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



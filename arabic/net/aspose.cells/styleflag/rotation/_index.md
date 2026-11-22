---
title: "StyleFlag.Rotation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعداد الدوران"
type: docs
url: /ar/net/aspose.cells/styleflag/rotation/
---
## StyleFlag.Rotation property

سيتم تطبيق إعداد الدوران.

```csharp
public bool Rotation { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyRotationDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية A1 وتعيين بعض النص
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Rotated Text");

            // احصل على نمط الخلية
            Style style = workbook.CreateStyle();

            // تعيين قيمة دوران جديدة (45 درجة)
            style.RotationAngle = 45;

            // عرض قيمة الدوران الحالية
            Console.WriteLine("Current Rotation value: " + cell.GetStyle().RotationAngle);            

            // إنشاء علامة نمط وتمكين علامة الدوران
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Rotation = true;

            // تطبيق النمط مع الدوران على الخلية
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("after setting style, rotation value: " + cell.GetStyle().RotationAngle);
           
            // حفظ النتيجة
            workbook.Save("PropertyRotationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



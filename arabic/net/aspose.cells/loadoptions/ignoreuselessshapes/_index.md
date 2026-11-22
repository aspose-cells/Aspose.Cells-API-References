---
title: "LoadOptions.IgnoreUselessShapes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تشير إلى ما إذا كان يتم تجاهل الأشكال غير المفيدة"
type: docs
url: /ar/net/aspose.cells/loadoptions/ignoreuselessshapes/
---
## LoadOptions.IgnoreUselessShapes property

يشير إلى ما إذا كان سيتم تجاهل الأشكال غير المفيدة.

```csharp
public bool IgnoreUselessShapes { get; set; }
```

### ملاحظات

يعمل فقط مع ملفات xlsx، xlsb، و xlsm. هناك العديد من الأشكال المتداخلة المتطابقة التي لا فائدة منها في بعض الملفات، يمكننا تجاهلها عند تحميل الملفات.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreUselessShapesDemo
    {
        public static void Run()
        {
            // إنشاء خيارات التحميل وتعيين IgnoreUselessShapes إلى true
            LoadOptions options = new LoadOptions();
            options.IgnoreUselessShapes = true;

            // حمّل دفتر العمل باستخدام الخيارات
            Workbook workbook = new Workbook("example.xlsx", options);

            // إخراج عدد الأشكال في ورقة العمل الأولى
            Console.WriteLine("Shapes count: " + workbook.Worksheets[0].Shapes.Count);
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



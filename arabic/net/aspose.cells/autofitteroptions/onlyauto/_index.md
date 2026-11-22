---
title: "AutoFitterOptions.OnlyAuto"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoFitterOptions. تشير إلى ما إذا كان سيتم ضبط الصفوف فقط التي لم يتم تخصيص ارتفاعها"
type: docs
url: /ar/net/aspose.cells/autofitteroptions/onlyauto/
---
## AutoFitterOptions.OnlyAuto property

يوضح ما إذا كان يتم ضبط الصفوف فقط التي ليس ارتفاعها مخصصًا.

```csharp
public bool OnlyAuto { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyOnlyAutoDemo
    {
        public static void Run()
        {
            // إنشاء خيارات التحميل وتعيين خاصية OnlyAuto
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = new AutoFitterOptions();
            loadOptions.AutoFitterOptions.OnlyAuto = true;

            // تحميل دفتر العمل مع خيارات الضبط التلقائي
            Workbook workbook = new Workbook("example.xml", loadOptions);
            
            // عرض الضبط التلقائي عن طريق فحص عرض العمود
            Console.WriteLine("Column width after auto-fit: " + 
                workbook.Worksheets[0].Cells.GetColumnWidthPixel(0));
            
            // احفظ وأعد التحميل للتحقق من الاستمرارية
            workbook.Save("example_output.xlsx");
            Workbook reloaded = new Workbook("example_output.xlsx");
            Console.WriteLine("Reloaded column width: " + 
                reloaded.Worksheets[0].Cells.GetColumnWidthPixel(0));
        }
    }
}
```

### انظر أيضًا

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



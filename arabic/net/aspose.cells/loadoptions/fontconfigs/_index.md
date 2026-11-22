---
title: "LoadOptions.FontConfigs"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تحصل وتعيّن تكوينات الخط الفردية. تعمل فقط مع المصنف الذي يستخدم هذه LoadOptions للتحميل"
type: docs
url: /ar/net/aspose.cells/loadoptions/fontconfigs/
---
## LoadOptions.FontConfigs property

تحصل وتعيّن تكوينات الخط الفردية. تعمل فقط مع الـ[`Workbook`](../../workbook/) الذي يستخدم هذه الـ[`LoadOptions`](../) للتحميل.

```csharp
public IndividualFontConfigs FontConfigs { get; set; }
```

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyFontConfigsDemo
    {
        public static void Run()
        {
            // أنشئ خيارات التحميل مع FontConfigs
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                FontConfigs = new IndividualFontConfigs()
            };

            // عيّن بعض قواعد استبدال الخط باستخدام الواجهة البرمجية الصحيحة
            loadOptions.FontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman" });
            loadOptions.FontConfigs.SetFontSubstitutes("Courier New", new string[] { "Consolas" });

            // تحميل ملف CSV باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("sample.csv", loadOptions);

            // حفظ المصنف إلى ملف Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [IndividualFontConfigs](../../individualfontconfigs/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



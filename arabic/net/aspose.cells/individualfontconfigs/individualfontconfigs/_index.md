---
title: "IndividualFontConfigs.IndividualFontConfigs"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ IndividualFontConfigs. Ctor"
type: docs
url: /ar/net/aspose.cells/individualfontconfigs/individualfontconfigs/
---
## IndividualFontConfigs constructor

منشئ.

```csharp
public IndividualFontConfigs()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IndividualFontConfigsMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء خيارات التحميل باستخدام IndividualFontConfigs
            var loadOptions = new OdsLoadOptions
            {
                FontConfigs = new IndividualFontConfigs(),
                StandardFont = "Arial",
                StandardFontSize = 12
            };

            // إنشاء مصنف جديد مع ورقة عمل افتراضية
            var workbook = new Workbook(FileFormatType.Xlsx);
            
            // الوصول إلى ورقة عمل وإضافة بعض النصوص
            var worksheet = workbook.Worksheets[0];
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text with custom font configs");

            // احفظ دفتر العمل (لا تحتاج خيارات التحميل للحفظ)
            workbook.Save("FontConfigsDemo.ods", SaveFormat.Ods);
        }
    }
}
```

### انظر أيضًا

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



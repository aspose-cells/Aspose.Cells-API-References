---
title: "NumbersLoadOptions.NumbersLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ NumbersLoadOptions. منشئ"
type: docs
url: /ar/net/aspose.cells.numbers/numbersloadoptions/numbersloadoptions/
---
## NumbersLoadOptions constructor

المُنشئ.

```csharp
public NumbersLoadOptions()
```

### أمثلة

```csharp
using System;
using System.Globalization;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء NumbersLoadOptions باستخدام المنشئ
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // تعيين بعض الخصائص الشائعة
                Password = "secure123",
                ParsingFormulaOnOpen = true,
                CultureInfo = new CultureInfo("en-US"),
                StandardFont = "Arial",
                MemorySetting = MemorySetting.MemoryPreference
            };

            // حمّل دفتر العمل باستخدام الخيارات
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // حفظ كـ XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)



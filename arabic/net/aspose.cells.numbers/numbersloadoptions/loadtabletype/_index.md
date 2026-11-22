---
title: "NumbersLoadOptions.LoadTableType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية NumbersLoadOptions. يحصل على ويضبط نوع تحميل جداول متعددة في ورقة عمل واحدة"
type: docs
url: /ar/net/aspose.cells.numbers/numbersloadoptions/loadtabletype/
---
## NumbersLoadOptions.LoadTableType property

الحصول على وتعيين نوع تحميل جداول متعددة في ورقة عمل واحدة.

```csharp
public LoadNumbersTableType LoadTableType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsPropertyLoadTableTypeDemo
    {
        public static void Run()
        {
            // إنشاء مثيل من NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // عرض كيفية استخدام خاصية LoadTableType
                LoadTableType = LoadNumbersTableType.OneTablePerSheet,
                
                // خصائص أخرى مطلوبة بالحد الأدنى
                Password = "password123",
                ParsingFormulaOnOpen = true
            };

            // تحميل ملف Numbers باستخدام خيارات التحميل المحددة
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // حفظ المصنف بتنسيق XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [LoadNumbersTableType](../../loadnumberstabletype/)
* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)



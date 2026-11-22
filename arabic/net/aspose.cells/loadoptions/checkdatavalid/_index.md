---
title: "LoadOptions.CheckDataValid"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تحقق مما إذا كانت البيانات صالحة في ملف القالب"
type: docs
url: /ar/net/aspose.cells/loadoptions/checkdatavalid/
---
## LoadOptions.CheckDataValid property

تحقق مما إذا كانت البيانات صالحة في ملف القالب.

```csharp
public bool CheckDataValid { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCheckDataValidDemo
    {
        public static void Run()
        {
            // أنشئ خيارات التحميل مع تعيين CheckDataValid إلى false
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            options.CheckDataValid = false;

            // حمّل المصنف باستخدام هذه الخيارات
            Workbook workbook = new Workbook("example.xlsx", options);

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض التحقق من صحة البيانات للتوضيح
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "100";

            // تعيين نطاق التحقق
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 10;
            area.EndColumn = 0;
            validation.AddArea(area);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "تعداد LoadNumbersTableType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Numbers.LoadNumbersTableType enum. يشير إلى نوع تحميل الجداول عندما تكون بعض الجداول في ورقة واحدة"
type: docs
url: /ar/net/aspose.cells.numbers/loadnumberstabletype/
---
## LoadNumbersTableType enumeration

يشير إلى نوع تحميل الجداول عندما تكون بعض الجداول في ورقة.

```csharp
public enum LoadNumbersTableType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| OneTablePerSheet | `1` |  |
| OverrideOtherTables | `2` |  |
| TileTables | `4` |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Numbers;
    using System;

    public class LoadNumbersTableTypeDemo
    {
        public static void LoadNumbersTableTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إنشاء ورقة عمل جديدة
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مثيل من NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions();

            // تعيين خاصية LoadNumbersTableType
            loadOptions.LoadTableType = LoadNumbersTableType.OneTablePerSheet;

            // تحميل ملف Numbers باستخدام خيارات التحميل المحددة
            workbook = new Workbook("LoadNumbersTableTypeExample_original.numbers", loadOptions);

            // حفظ المصنف إلى ملف Excel
            workbook.Save("LoadNumbersTableTypeExample.xlsx");

            Console.WriteLine("Workbook loaded and saved successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Numbers](../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../)



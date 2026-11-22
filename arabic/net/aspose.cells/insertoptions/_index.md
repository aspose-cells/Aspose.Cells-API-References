---
title: "الفئة InsertOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.InsertOptions. تمثل خيارات الإدراج"
type: docs
url: /ar/net/aspose.cells/insertoptions/
---
## InsertOptions class

يمثل خيارات الإدراج.

```csharp
public class InsertOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [InsertOptions](insertoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CopyFormatType](../../aspose.cells/insertoptions/copyformattype/) { get; set; } |  |
| [FormulaChangeMonitor](../../aspose.cells/insertoptions/formulachangemonitor/) { get; set; } | يحصل/يضبط المراقب لتتبع التغييرات الناجمة عن الإدراج. |
| [UpdateReference](../../aspose.cells/insertoptions/updatereference/) { get; set; } | يشير إلى ما إذا كانت المراجع في أوراق عمل أخرى سيتم تحديثها. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InsertOptionsDemo
    {
        public static void InsertOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء كائن من InsertOptions
            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // تحديد نطاق الخلايا حيث سيتم إدراج الصفوف
            CellArea cellArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };

            // إدراج الصفوف باستخدام الخيارات المحددة
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            // احفظ المصنف
            workbook.Save("InsertOptionsExample.xlsx");
            workbook.Save("InsertOptionsExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



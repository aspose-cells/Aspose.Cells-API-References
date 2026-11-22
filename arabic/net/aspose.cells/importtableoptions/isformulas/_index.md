---
title: "ImportTableOptions.IsFormulas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImportTableOptions. تشير إلى ما إذا كانت البيانات صيغًا"
type: docs
url: /ar/net/aspose.cells/importtableoptions/isformulas/
---
## ImportTableOptions.IsFormulas property

يشير إلى ما إذا كانت البيانات صيغًا.

```csharp
public bool[] IsFormulas { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyIsFormulasDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إنشاء جدول بيانات تجريبي بمحتوى صيغ
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1");
            dt.Rows.Add("=SUM(1,2,3)");
            dt.Rows.Add("=AVERAGE(4,5,6)");

            // تعيين خيارات الاستيراد مع خاصية IsFormulas
            ImportTableOptions options = new ImportTableOptions();
            options.IsFormulas = new bool[] { true }; // Treat first column as formulas
            
            // استيراد البيانات مع الصيغ
            workbook.Worksheets[0].Cells.ImportData(dt, 0, 0, options);

            // تحقق من أن الصيغ تم استيرادها بشكل صحيح
            Console.WriteLine("Cell A1 formula: " + workbook.Worksheets[0].Cells["A1"].Formula);
            Console.WriteLine("Cell A2 formula: " + workbook.Worksheets[0].Cells["A2"].Formula);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



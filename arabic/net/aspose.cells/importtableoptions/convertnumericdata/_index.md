---
title: "ImportTableOptions.ConvertNumericData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImportTableOptions. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب تحويل القيمة النصية إلى قيمة رقمية أو تاريخية"
type: docs
url: /ar/net/aspose.cells/importtableoptions/convertnumericdata/
---
## ImportTableOptions.ConvertNumericData property

يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب تحويل القيمة النصية إلى قيمة رقمية أو تاريخية.

```csharp
public bool ConvertNumericData { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إنشاء جدول بيانات تجريبي يحتوي على قيم رقمية ونصية
            DataTable dt = new DataTable();
            dt.Columns.Add("Numbers");
            dt.Columns.Add("Text");
            dt.Rows.Add("123", "456");
            dt.Rows.Add("ABC", "DEF");

            // الحصول على خلايا ورقة العمل الأولى
            Cells cells = workbook.Worksheets[0].Cells;

            // إنشاء خيارات الاستيراد مع تعيين ConvertNumericData إلى true
            ImportTableOptions options = new ImportTableOptions();
            options.ConvertNumericData = true;
            options.IsFieldNameShown = true;

            // استيراد البيانات مع التحويل الرقمي
            cells.ImportData(dt, 0, 0, options);

            // عرض النتائج
            Console.WriteLine("A2 (numeric converted): " + cells["A2"].Value + " - Type: " + cells["A2"].Type);
            Console.WriteLine("B2 (string remains): " + cells["B2"].StringValue + " - Type: " + cells["B2"].Type);
        }
    }
}
```

### انظر أيضًا

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



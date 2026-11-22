---
title: "ImportTableOptions.DateFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImportTableOptions. تحصل أو تعين سلسلة تنسيق التاريخ للخلايا التي تحتوي على قيم تاريخ ووقت مستوردة"
type: docs
url: /ar/net/aspose.cells/importtableoptions/dateformat/
---
## ImportTableOptions.DateFormat property

يحصل أو يضبط سلسلة تنسيق التاريخ للخلايا التي تحتوي على قيم تاريخ ووقت مستوردة.

```csharp
public string DateFormat { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء DataTable تجريبي يحتوي على قيم تاريخ
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("DateColumn", typeof(DateTime));
            dataTable.Rows.Add(new DateTime(2023, 1, 15));
            dataTable.Rows.Add(new DateTime(2023, 2, 20));
            dataTable.Rows.Add(new DateTime(2023, 3, 25));

            // تحديد نطاق الاستيراد
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 10, 1);

            // استيراد البيانات باستخدام تنسيق تاريخ مخصص
            worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions()
            {
                IsFieldNameShown = true,
                DateFormat = "YYYY-MM-DD"
            });

            // احفظ المصنف لعرض النتيجة
            workbook.Save("DateFormatDemoOutput.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "ImportTableOptions.TotalRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImportTableOptions. تحصل أو تعين عدد الصفوف الإجمالي للاستيراد من مصدر البيانات. 1 يعني جميع الصفوف في مصدر البيانات المحدد"
type: docs
url: /ar/net/aspose.cells/importtableoptions/totalrows/
---
## ImportTableOptions.TotalRows property

يحصل أو يضبط العدد الإجمالي للصفوف للاستيراد من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد.

```csharp
public int TotalRows { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalRowsDemo
    {
        public static void Run()
        {
            // أنشئ DataTable نموذجية
            DataTable table = new DataTable("TestTable");
            table.Columns.Add("Column1", typeof(string));
            table.Columns.Add("Column2", typeof(int));
            
            // أضف بيانات تجريبية
            table.Rows.Add("Item1", 100);
            table.Rows.Add("Item2", 200);
            table.Rows.Add("Item3", 300);

            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء ImportTableOptions مع تعيين TotalRows إلى 2 (سيتم استيراد الصفين الأولين فقط)
            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalRows = 2 // Only import 2 rows from the DataTable
            };

            // استيراد البيانات باستخدام الخيارات المحددة
            worksheet.Cells.ImportData(table, 0, 0, options);

            // احفظ المصنف
            workbook.Save("ImportWithTotalRows.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Data imported with TotalRows=2. Only first 2 rows were imported.");
        }
    }
}
```

### انظر أيضًا

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



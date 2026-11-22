---
title: "ExportTableOptions.PlotVisibleRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExportTableOptions. تصدر فقط الصفوف الظاهرة"
type: docs
url: /ar/net/aspose.cells/exporttableoptions/plotvisiblerows/
---
## ExportTableOptions.PlotVisibleRows property

يصدّر فقط الصفوف المرئية.

```csharp
public bool PlotVisibleRows { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyPlotVisibleRowsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف والوصول إلى ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء بيانات عينة في ورقة العمل
            cells["A1"].PutValue("Column1");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);
            cells["A4"].PutValue(30);

            // إخفاء الصف 3 (الفهرس 2) الذي يحتوي على القيمة 20
            worksheet.Cells.HideRow(2);

            // إنشاء DataTable للتصدير إليه
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Column1", typeof(int));

            // إعداد خيارات التصدير
            ExportTableOptions options = new ExportTableOptions();
            options.PlotVisibleRows = true; // Only export visible rows
            options.ExportColumnName = true;
            options.DataTable = dataTable;

            // تصدير البيانات (يجب تخطي الصف المخفي)
            cells.ExportDataTable(0, 0, 4, 1, options);

            // عرض البيانات المصدرة
            Console.WriteLine("Exported Data (PlotVisibleRows=true):");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine(row["Column1"]);
            }
        }
    }
}
```

### انظر أيضًا

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



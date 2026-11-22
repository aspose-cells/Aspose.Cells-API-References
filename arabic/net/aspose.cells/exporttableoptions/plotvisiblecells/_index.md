---
title: "ExportTableOptions.PlotVisibleCells"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExportTableOptions. تصدر فقط الخلايا الظاهرة"
type: docs
url: /ar/net/aspose.cells/exporttableoptions/plotvisiblecells/
---
## ExportTableOptions.PlotVisibleCells property

يصدّر فقط الخلايا المرئية.

```csharp
public bool PlotVisibleCells { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyPlotVisibleCellsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة مع بعض الصفوف/الأعمدة المخفية
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");
            
            // إخفاء الصف 2 والعمود B (الفهرس 1)
            worksheet.Cells.HideRow(1);
            worksheet.Cells.HideColumn(1);

            // إنشاء خيارات التصدير مع تعيين PlotVisibleCells إلى true
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                PlotVisibleCells = true,
                PlotVisibleColumns = true,
                PlotVisibleRows = true
            };

            // تصدير الخلايا الظاهرة فقط
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 3, exportOptions);

            // عرض البيانات المصدرة (يجب تصدير الخلايا الظاهرة فقط)
            Console.WriteLine("Exported Data:");
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### انظر أيضًا

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "ExportTableOptions.ExportAsHtmlString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExportTableOptions. تصدّر القيمة النصية HTML للخلايا إلى DataTable"
type: docs
url: /ar/net/aspose.cells/exporttableoptions/exportashtmlstring/
---
## ExportTableOptions.ExportAsHtmlString property

يصدّر قيمة سلسلة HTML للخلايا إلى DataTable.

```csharp
public bool ExportAsHtmlString { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyExportAsHtmlStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // تعيين قيمة الخلية مع التنسيق
            cells["A1"].PutValue("abc");
            Style style = cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.Font.Color = System.Drawing.Color.Black;
            cells["A1"].SetStyle(style);

            // تصدير مع ExportAsHtmlString
            ExportTableOptions etOpt = new ExportTableOptions();
            etOpt.ExportColumnName = false;
            etOpt.ExportAsHtmlString = true;
            
            DataTable dt = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            
            Console.WriteLine("HTML String: " + dt.Rows[0][0].ToString());
            Console.WriteLine("Expected Format: " + cells["A1"].HtmlString);
        }
    }
}
```

### انظر أيضًا

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



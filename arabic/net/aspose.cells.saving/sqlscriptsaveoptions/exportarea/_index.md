---
title: "SqlScriptSaveOptions.ExportArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SqlScriptSaveOptions. تحصل أو تعيين نطاق التصدير"
type: docs
url: /ar/net/aspose.cells.saving/sqlscriptsaveoptions/exportarea/
---
## SqlScriptSaveOptions.ExportArea property

يحصل أو يعيّن نطاق التصدير.

```csharp
public CellArea ExportArea { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء ورقة العمل ببيانات عينة
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // تكوين خيارات تصدير SQL مع ExportArea
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                ExportArea = new CellArea { StartRow = 0, EndRow = 3, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true
            };

            // حفظ مع نطاق تصدير محدد (الأعمدة A1:B3)
            workbook.Save("EmployeesExport.sql", saveOptions);
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)



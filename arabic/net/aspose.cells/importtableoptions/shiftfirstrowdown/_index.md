---
title: "ImportTableOptions.ShiftFirstRowDown"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImportTableOptions. تشير إلى ما إذا كان يتم إزاحة الصف الأول إلى الأسفل عند إدراج الصفوف"
type: docs
url: /ar/net/aspose.cells/importtableoptions/shiftfirstrowdown/
---
## ImportTableOptions.ShiftFirstRowDown property

يشير إلى ما إذا كان يتم إزاحة الصف الأول إلى الأسفل عند إدراج الصفوف.

```csharp
public bool ShiftFirstRowDown { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyShiftFirstRowDownDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // إنشاء DataTable نموذجي
            DataTable table = new DataTable();
            table.Columns.Add("Column1");
            table.Columns.Add("Column2");
            table.Rows.Add("Header1", "Header2");
            table.Rows.Add("Data1", "Data2");
            table.Rows.Add("Data3", "Data4");

            // استيراد مع ShiftFirstRowDown = false (السلوك الافتراضي)
            var options1 = new ImportTableOptions
            {
                IsFieldNameShown = false,
                ShiftFirstRowDown = false
            };
            cells.ImportData(table, 0, 0, options1);
            Console.WriteLine("With ShiftFirstRowDown=false, first row starts at A1: " + cells[0, 0].StringValue);

            // مسح ورقة العمل واستيراد مع ShiftFirstRowDown = true
            workbook.Worksheets[0].Cells.Clear();
            var options2 = new ImportTableOptions
            {
                IsFieldNameShown = false,
                ShiftFirstRowDown = true
            };
            cells.ImportData(table, 0, 0, options2);
            Console.WriteLine("With ShiftFirstRowDown=true, first row is shifted down to A2: " + cells[1, 0].StringValue);

            // احفظ المصنف
            workbook.Save("ShiftFirstRowDownDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



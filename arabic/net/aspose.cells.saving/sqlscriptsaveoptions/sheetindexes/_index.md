---
title: "SqlScriptSaveOptions.SheetIndexes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SqlScriptSaveOptions. تمثل فهارس الأوراق المصدرة"
type: docs
url: /ar/net/aspose.cells.saving/sqlscriptsaveoptions/sheetindexes/
---
## SqlScriptSaveOptions.SheetIndexes property

يمثل فهارس الأوراق المصدرة.

```csharp
public int[] SheetIndexes { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد يحتوي على عدة أوراق
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // ملء بعض البيانات في جميع الأوراق
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet worksheet = workbook.Worksheets[i];
                worksheet.Cells["A1"].PutValue("ID");
                worksheet.Cells["B1"].PutValue("Name");
                worksheet.Cells["A2"].PutValue(1);
                worksheet.Cells["B2"].PutValue("John");
                worksheet.Cells["A3"].PutValue(2);
                worksheet.Cells["B3"].PutValue("Jane");
            }

            // إنشاء كائن SqlScriptSaveOptions
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // عرض SheetIndexes الحالية (null يعني جميع الأوراق)
            Console.WriteLine("Initial SheetIndexes: " + 
                (options.SheetIndexes == null ? "All sheets" : string.Join(",", options.SheetIndexes)));

            // ضبط SheetIndexes لتصدير الورقتين الأولى والثالثة فقط (0 و 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // حفظ باستخدام الخيارات
            workbook.Save("SqlScriptExportSelectedSheets.sql", options);

            // تغيير SheetIndexes لتصدير الورقة الثانية فقط
            options.SheetIndexes = new int[] { 1 };
            workbook.Save("SqlScriptExportSecondSheet.sql", options);

            // تعيين SheetIndexes إلى فارغ لتصدير جميع الأوراق
            options.SheetIndexes = null;
            workbook.Save("SqlScriptExportAllSheets.sql", options);
        }
    }
}
```

### انظر أيضًا

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)



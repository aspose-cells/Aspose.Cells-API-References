---
title: "ImportTableOptions.InsertRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImportTableOptions. تشير إلى ما إذا كان يجب إضافة صفوف جديدة لاستيراد سجلات البيانات"
type: docs
url: /ar/net/aspose.cells/importtableoptions/insertrows/
---
## ImportTableOptions.InsertRows property

يشير إلى ما إذا كان يجب إضافة صفوف جديدة لاستيراد سجلات البيانات.

```csharp
public bool InsertRows { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyInsertRowsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء جدول بيانات تجريبي
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            dataTable.Rows.Add(1, "Laptop", 999.99);
            dataTable.Rows.Add(2, "Monitor", 249.99);
            dataTable.Rows.Add(3, "Keyboard", 49.99);

            // إضافة البيانات الحالية إلى ورقة العمل (سيتم إزاحتها إلى الأسفل بواسطة الإدراج)
            cells["A1"].PutValue("Existing Data");
            cells["A2"].PutValue(100);

            // تعيين خيارات الاستيراد مع InsertRows = true
            ImportTableOptions options = new ImportTableOptions();
            options.InsertRows = true; // This will insert new rows instead of overwriting
            options.IsFieldNameShown = true;

            // استيراد البيانات بدءًا من الصف 1 (سيتم إدراج صفوف أسفل البيانات الحالية)
            cells.ImportData(dataTable, 1, 0, options);

            // احفظ المصنف
            workbook.Save("InsertRowsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



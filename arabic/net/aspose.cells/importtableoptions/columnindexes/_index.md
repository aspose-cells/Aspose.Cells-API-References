---
title: "ImportTableOptions.ColumnIndexes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImportTableOptions. يحصل أو يضبط الأعمدة ذات الفهرس 0 لاستيرادها من مصدر البيانات. null يعني أنه يجب استيراد جميع الأعمدة"
type: docs
url: /ar/net/aspose.cells/importtableoptions/columnindexes/
---
## ImportTableOptions.ColumnIndexes property

يحصل أو يضبط الأعمدة (بدءًا من الصفر) للاستيراد من مصدر البيانات. يعني null أنه يجب استيراد جميع الأعمدة.

```csharp
public int[] ColumnIndexes { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyColumnIndexesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء DataTable نموذجي
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // أضف بيانات تجريبية
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);
            dataTable.Rows.Add(3, "Product C", 39.99m);

            // ضبط خيارات الاستيراد لاستيراد الأعمدة فقط في الفهارس 0 و 2 (ID و Price)
            ImportTableOptions options = new ImportTableOptions();
            options.ColumnIndexes = new int[] { 0, 2 };
            options.IsFieldNameShown = true;

            // استيراد البيانات باستخدام فهارس الأعمدة المحددة
            worksheet.Cells.ImportData(dataTable, 0, 0, options);

            // احفظ المصنف
            workbook.Save("ColumnIndexesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



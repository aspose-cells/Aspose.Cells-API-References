---
title: "ImportTableOptions.ConvertGridStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImportTableOptions. تشير إلى ما إذا كان يتم تطبيق نمط عرض الشبكة على الخلايا"
type: docs
url: /ar/net/aspose.cells/importtableoptions/convertgridstyle/
---
## ImportTableOptions.ConvertGridStyle property

يشير إلى ما إذا كان يتم تطبيق نمط عرض الشبكة على الخلايا.

```csharp
public bool ConvertGridStyle { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyConvertGridStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات نموذجية
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            dataTable.Rows.Add(101, "Laptop", 999.99m);
            dataTable.Rows.Add(102, "Monitor", 249.50m);

            // تعيين خيارات الاستيراد مع تمكين ConvertGridStyle
            ImportTableOptions options = new ImportTableOptions();
            options.ConvertGridStyle = true; // This will apply grid styling to the imported data
            options.IsFieldNameShown = true;

            // استيراد البيانات مع التنسيق
            worksheet.Cells.ImportData(dataTable, 0, 0, options);

            // حفظ النتيجة
            workbook.Save("ImportWithGridStyle.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



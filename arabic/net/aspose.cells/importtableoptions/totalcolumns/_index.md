---
title: "ImportTableOptions.TotalColumns"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImportTableOptions. تحصل أو تعين عدد الأعمدة الكلية للاستيراد من مصدر البيانات. 1 يعني جميع الصفوف في مصدر البيانات المحدد"
type: docs
url: /ar/net/aspose.cells/importtableoptions/totalcolumns/
---
## ImportTableOptions.TotalColumns property

يحصل أو يضبط العدد الإجمالي للأعمدة للاستيراد من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد.

```csharp
public int TotalColumns { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalColumnsDemo
    {
        public static void Run()
        {
            // أنشئ DataTable نموذجية
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // أضف بيانات تجريبية
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين خيارات الاستيراد مع TotalColumns = 2 (سيتم استيراد أول عمودين فقط)
            ImportTableOptions importOptions = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalColumns = 2 // Only import first 2 columns (ID and Name)
            };

            // استيراد البيانات بدءًا من الخلية A1
            cells.ImportData(dataTable, 0, 0, importOptions);

            // احفظ المصنف
            workbook.Save("ImportWithTotalColumns.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Data imported with TotalColumns=2. Only first 2 columns were imported.");
        }
    }
}
```

### انظر أيضًا

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



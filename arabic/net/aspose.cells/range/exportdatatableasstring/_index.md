---
title: "Range.ExportDataTableAsString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تصدر البيانات في هذا النطاق إلى كائن DataTable"
type: docs
url: /ar/net/aspose.cells/range/exportdatatableasstring/
---
## Range.ExportDataTableAsString method

يصدّر البيانات في هذا النطاق إلى كائن DataTable.

```csharp
public DataTable ExportDataTableAsString()
```

### قيمة الإرجاع

كائن DataTable المُصدّر.

### ملاحظات

جميع البيانات في مجموعة [`Cells`](../../cells/) تُحوَّل إلى سلاسل.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class RangeMethodExportDataTableAsStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(30);

            // احصل على النطاق الذي يحتوي على البيانات
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            try
            {
                // استدعِ طريقة ExportDataTableAsString
                DataTable dataTable = range.ExportDataTableAsString();

                // عرض البيانات المصدرة
                Console.WriteLine("Exported DataTable:");
                foreach (DataRow row in dataTable.Rows)
                {
                    Console.WriteLine($"{row[0]}, {row[1]}");
                }

                // احفظ المصنف
                workbook.Save("RangeMethodExportDataTableAsStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ExportDataTableAsString method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



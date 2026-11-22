---
title: "ExportTableOptions.FormatStrategy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExportTableOptions. تحصل وتعيّن استراتيجية التنسيق عند تصدير القيمة كقيمة نصية"
type: docs
url: /ar/net/aspose.cells/exporttableoptions/formatstrategy/
---
## ExportTableOptions.FormatStrategy property

يحصل ويضبط استراتيجية التنسيق عند تصدير القيمة كقيمة سلسلة.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### ملاحظات

القيمة الافتراضية هي CellStyle.

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية مع التنسيق
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            Style styleB2 = worksheet.Cells["B2"].GetStyle();
            styleB2.Number = 4; // Currency format
            worksheet.Cells["B2"].SetStyle(styleB2);
            
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(599.99);
            Style styleB3 = worksheet.Cells["B3"].GetStyle();
            styleB3.Number = 4; // Currency format
            worksheet.Cells["B3"].SetStyle(styleB3);

            // إنشاء خيارات تصدير باستراتيجيات تنسيق مختلفة
            ExportTableOptions optionsDisplayStyle = new ExportTableOptions
            {
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                ExportColumnName = true
            };

            ExportTableOptions optionsCellStyle = new ExportTableOptions
            {
                FormatStrategy = CellValueFormatStrategy.CellStyle,
                ExportColumnName = true
            };

            // تصدير باستخدام استراتيجيات مختلفة
            Console.WriteLine("DisplayStyle Format Strategy:");
            DataTable dtDisplay = worksheet.Cells.ExportDataTable(0, 0, 3, 2, optionsDisplayStyle);
            PrintDataTable(dtDisplay);

            Console.WriteLine("\nCellStyle Format Strategy:");
            DataTable dtCellStyle = worksheet.Cells.ExportDataTable(0, 0, 3, 2, optionsCellStyle);
            PrintDataTable(dtCellStyle);
        }

        private static void PrintDataTable(DataTable dt)
        {
            foreach (DataRow row in dt.Rows)
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

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



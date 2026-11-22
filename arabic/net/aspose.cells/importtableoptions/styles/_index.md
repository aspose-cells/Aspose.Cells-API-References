---
title: "ImportTableOptions.Styles"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImportTableOptions. يحصل على الأنماط ويضبطها لكل عمود في الجدول"
type: docs
url: /ar/net/aspose.cells/importtableoptions/styles/
---
## ImportTableOptions.Styles property

يحصل ويضبط الأنماط لكل عمود في الجدول.

```csharp
public Style[] Styles { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsPropertyStylesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء جدول بيانات تجريبي
            DataTable dt = new DataTable();
            dt.Columns.Add("Product");
            dt.Columns.Add("Price");
            dt.Rows.Add("Apple", 1.50);
            dt.Rows.Add("Banana", 0.75);
            dt.Rows.Add("Orange", 1.20);

            try
            {
                // إنشاء ImportTableOptions وتعيين خاصية Styles
                ImportTableOptions options = new ImportTableOptions();
                options.IsFieldNameShown = true;

                // إنشاء أنماط لكل عمود
                Style[] columnStyles = new Style[2];

                // نمط لعمود المنتج (عريض، خط أزرق)
                Style productStyle = workbook.CreateStyle();
                productStyle.Font.IsBold = true;
                productStyle.Font.Color = System.Drawing.Color.Blue;
                columnStyles[0] = productStyle;

                // نمط لعمود السعر (تنسيق عملة، خط أخضر)
                Style priceStyle = workbook.CreateStyle();
                priceStyle.Font.Color = System.Drawing.Color.Green;
                priceStyle.Number = 4; // Currency format
                columnStyles[1] = priceStyle;

                // تعيين خاصية Styles
                options.Styles = columnStyles;

                // استيراد البيانات مع الأنماط
                worksheet.Cells.ImportData(dt, 0, 0, options);

                // عرض الأنماط المطبقة
                Console.WriteLine("Styles applied to columns:");
                Console.WriteLine($"Product column style: Bold={columnStyles[0].Font.IsBold}, Color={columnStyles[0].Font.Color.Name}");
                Console.WriteLine($"Price column style: NumberFormat={columnStyles[1].Number}, Color={columnStyles[1].Font.Color.Name}");

                // احفظ المصنف
                workbook.Save("StylesDemo.xlsx");
                Console.WriteLine("Workbook saved with styled data.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "JsonSaveOptions.ExportStylePool"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonSaveOptions. تشير إلى ما إذا كان سيتم تصدير الأنماط جماعياً أو فردياً لكل خلية"
type: docs
url: /ar/net/aspose.cells/jsonsaveoptions/exportstylepool/
---
## JsonSaveOptions.ExportStylePool property

يشير إلى ما إذا كان يتم تصدير الأنماط بشكل جماعي أو فردي لكل خلية.

```csharp
public bool ExportStylePool { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonSaveOptionsPropertyExportStylePoolDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية بأنماط مختلفة
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);

            // تطبيق أنماط مختلفة على الخلايا
            Aspose.Cells.Style style1 = workbook.CreateStyle();
            style1.Font.Color = System.Drawing.Color.Red;
            worksheet.Cells["A1"].SetStyle(style1);

            Aspose.Cells.Style style2 = workbook.CreateStyle();
            style2.Font.Color = System.Drawing.Color.Blue;
            worksheet.Cells["B1"].SetStyle(style2);

            try
            {
                // إنشاء JsonSaveOptions مع ExportStylePool = true (تصدير جماعي)
                JsonSaveOptions options1 = new JsonSaveOptions();
                options1.ExportStylePool = true;
                Console.WriteLine("ExportStylePool (collective): " + options1.ExportStylePool);

                // حفظ مع تصدير الأنماط الجماعي
                workbook.Save("output_collective_styles.json", options1);

                // إنشاء JsonSaveOptions مع ExportStylePool = false (تصدير فردي)
                JsonSaveOptions options2 = new JsonSaveOptions();
                options2.ExportStylePool = false;
                Console.WriteLine("ExportStylePool (individual): " + options2.ExportStylePool);

                // حفظ مع تصدير الأنماط الفردي
                workbook.Save("output_individual_styles.json", options2);

                Console.WriteLine("ExportStylePool demonstration completed successfully.");
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

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



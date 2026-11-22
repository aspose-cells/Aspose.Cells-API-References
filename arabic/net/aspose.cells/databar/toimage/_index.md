---
title: "DataBar.ToImage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة DataBar. قم بتحويل شريط البيانات في الخلية إلى مصفوفة بايت للصورة"
type: docs
url: /ar/net/aspose.cells/databar/toimage/
---
## DataBar.ToImage method

قم بتحويل شريط البيانات في الخلية إلى مصفوفة بايت للصورة.

```csharp
public byte[] ToImage(Cell cell, ImageOrPrintOptions imgOpts)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خلية | خلية | حدد الخلية التي سيُعرض فيها شريط البيانات |
| imgOpts | ImageOrPrintOptions | ImageOrPrintOptions يحتوي على بعض خصائص صورة الإخراج |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class DataBarMethodToImageWithCellImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة وتنسيق شرطي
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            
            // إضافة تنسيق شرطي لشريط البيانات
            int idx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);
            
            idx = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcc[idx];
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            
            // احصل على الخلية التي تحتوي على تنسيق شرطي
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
            
            if (result != null && result.ConditionalFormattingDataBar != null)
            {
                DataBar bar = result.ConditionalFormattingDataBar;
                ImageOrPrintOptions imgOpts = new ImageOrPrintOptions();
                
                // حوّل شريط البيانات إلى صورة
                byte[] img = bar.ToImage(cell, imgOpts);
                
                // احفظ الصورة
                string outputPath = "DataBarImage.png";
                File.WriteAllBytes(outputPath, img);
                
                // للتحقق من الصورة، ستحتاج إلى إضافة حزمة System.Drawing.Common
                // واستخدم System.Drawing.Image إذا لزم الأمر
                Console.WriteLine($"Data bar image saved to {outputPath}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



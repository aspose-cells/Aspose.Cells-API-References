---
title: "ImageOrPrintOptions.AllColumnsInOnePagePerSheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. إذا كان AllColumnsInOnePagePerSheet صحيحًا، سيتم إخراج جميع محتوى الأعمدة لورقة واحدة في صفحة واحدة فقط في النتيجة. سيكون عرض حجم الورق في إعدادات الصفحة غير صالح وستظل الإعدادات الأخرى لإعدادات الصفحة سارية."
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/
---
## ImageOrPrintOptions.AllColumnsInOnePagePerSheet property

إذا كان AllColumnsInOnePagePerSheet صحيحًا، فسيتم إخراج جميع محتويات الأعمدة لورقة واحدة في صفحة واحدة فقط في النتيجة. سيكون عرض حجم الورق في إعداد الصفحة غير صالح، وستظل الإعدادات الأخرى لإعداد الصفحة سارية.

```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyAllColumnsInOnePagePerSheetDemo
    {
        public static void Run()
        {
            // إنشاء مصنف وإضافة بيانات نموذجية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء بعض البيانات في ورقة العمل
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // إنشاء خيارات حفظ الصورة
            ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
            pngOptions.ImageOrPrintOptions.AllColumnsInOnePagePerSheet = true;
            pngOptions.ImageOrPrintOptions.OnePagePerSheet = true;

            // احفظ دفتر العمل إلى تدفق الذاكرة بصيغة PNG
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, pngOptions);
                Console.WriteLine("Workbook saved as PNG with all columns in one page per sheet.");
            }
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



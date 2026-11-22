---
title: "FontSetting.SetWordArtStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FontSetting. تعيين نمط WordArt المسبق"
type: docs
url: /ar/net/aspose.cells/fontsetting/setwordartstyle/
---
## FontSetting.SetWordArtStyle method

يضبط نمط WordArt المسبق.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | PresetWordArtStyle | نمط WordArt المسبق. |

### ملاحظات

فقط لنص الشكل/المخطط.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class FontSettingMethodSetWordArtStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض النص إلى الخلية A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text for WordArt");

            // إنشاء إعداد الخط للنص في الخلية A1
            FontSetting fontSetting = new FontSetting(0, cell.StringValue.Length, workbook.Worksheets);

            try
            {
                // تطبيق نمط WordArt على إعداد الخط
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle3);

                Console.WriteLine("WordArt style applied successfully to the text.");
                
                // عرض التأثير عن طريق حفظ المصنف
                worksheet.AutoFitColumn(0);
                worksheet.AutoFitRow(0);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("FontSettingMethodSetWordArtStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



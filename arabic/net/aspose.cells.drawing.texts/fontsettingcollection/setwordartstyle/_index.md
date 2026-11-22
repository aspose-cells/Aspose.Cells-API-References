---
title: "FontSettingCollection.SetWordArtStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FontSettingCollection. تعيين نمط WordArt المسبق"
type: docs
url: /ar/net/aspose.cells.drawing.texts/fontsettingcollection/setwordartstyle/
---
## FontSettingCollection.SetWordArtStyle method

يضبط نمط WordArt المسبق.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | PresetWordArtStyle | نمط WordArt المسبق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodSetWordArtStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // حدد النص الأولي
            fontSettingCollection.Text = "Sample Text for WordArt Styling";

            try
            {
                // استدعِ طريقة SetWordArtStyle مع WordArtStyle7 (تعبئة متدرجة - أزرق، تمييز 1، انعكاس)
                fontSettingCollection.SetWordArtStyle(PresetWordArtStyle.WordArtStyle7);

                Console.WriteLine("WordArt style applied successfully to the text box.");

                // احفظ المصنف لإظهار التأثير
                workbook.Save("FontSettingCollectionSetWordArtStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



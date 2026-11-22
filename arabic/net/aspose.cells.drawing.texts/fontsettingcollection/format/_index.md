---
title: "FontSettingCollection.Format"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FontSettingCollection. تنسيق النص باستخدام إعداد الخط"
type: docs
url: /ar/net/aspose.cells.drawing.texts/fontsettingcollection/format/
---
## FontSettingCollection.Format method

نسق النص باستخدام إعداد الخط.

```csharp
public void Format(int startIndex, int length, Font font, StyleFlag flag)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | Int32 | فهرس البداية. |
| الطول | Int32 | الطول. |
| خط | خط | الخط. |
| علامة | StyleFlag | علامات الخط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodFormatWithInt32Int32FontStyleFlagDemo
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
            fontSettingCollection.Text = "Sample Text for Formatting";

            try
            {
                // إنشاء نمط وتعيين خصائص الخط الخاصة به
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                style.Font.IsBold = true;
                style.Font.Color = System.Drawing.Color.Red;

                // إنشاء علامة النمط لتحديد خصائص الخط التي سيتم تطبيقها
                StyleFlag styleFlag = new StyleFlag();
                styleFlag.FontName = true;
                styleFlag.FontSize = true;
                styleFlag.FontBold = true;
                styleFlag.FontColor = true;

                // تنسيق الأحرف من الفهرس 7 إلى 11 (الكلمة "Text")
                fontSettingCollection.Format(7, 4, style.Font, styleFlag);

                // احفظ المصنف لإظهار التأثير
                workbook.Save("FontSettingCollectionFormatDemo.xlsx");
                Console.WriteLine("Format method executed successfully. Text 'Text' is now bold, red Arial 14pt.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Format method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



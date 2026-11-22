---
title: "IndividualFontConfigs.SetFontSubstitutes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة IndividualFontConfigs. تقوم بتعيين أسماء بدائل الخط لاسم الخط الأصلي المحدد"
type: docs
url: /ar/net/aspose.cells/individualfontconfigs/setfontsubstitutes/
---
## IndividualFontConfigs.SetFontSubstitutes method

يضبط أسماء بدائل الخط لاسم خط أصلي معين.

```csharp
public void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| originalFontName | String | اسم الخط الأصلي. |
| substituteFontNames | String[] | قائمة بأسماء بدائل الخط التي تُستخدم إذا لم يُقدَّم الخط الأصلي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء نسخة من IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // اسم الخط الأصلي وبدائله
            string originalFont = "Arial";
            string[] substitutes = new string[] { "Helvetica", "Verdana", "Times New Roman" };

            try
            {
                // استدعِ SetFontSubstitutes مع المعلمات المحددة
                fontConfigs.SetFontSubstitutes(originalFont, substitutes);

                Console.WriteLine($"Successfully set font substitutes for '{originalFont}'");
                Console.WriteLine("Substitutes are:");
                foreach (var sub in substitutes)
                {
                    Console.WriteLine($"- {sub}");
                }

                // أنشئ دفتر عمل لتوضيح التأثير
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // تعيين نمط باستخدام الخط الأصلي
                Style style = workbook.CreateStyle();
                style.Font.Name = originalFont;
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].Value = "This text uses " + originalFont;
                worksheet.Cells["A1"].SetStyle(style);

                // احفظ المصنف
                workbook.Save("FontSubstitutesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font substitutes: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



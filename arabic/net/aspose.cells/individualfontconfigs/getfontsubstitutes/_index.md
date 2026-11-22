---
title: "IndividualFontConfigs.GetFontSubstitutes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة IndividualFontConfigs. تُرجع مصفوفة تحتوي على أسماء بدائل الخط لتُستخدم إذا لم يُقدم الخط الأصلي"
type: docs
url: /ar/net/aspose.cells/individualfontconfigs/getfontsubstitutes/
---
## IndividualFontConfigs.GetFontSubstitutes method

يعيد مصفوفة تحتوي على أسماء بدائل الخط لاستخدامها إذا لم يتوفر الخط الأصلي.

```csharp
public string[] GetFontSubstitutes(string originalFontName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| originalFontName | String | originalFontName |

### قيمة الإرجاع

مصفوفة تحتوي على أسماء بدائل الخط لاستخدامها إذا لم يكن الخط الأصلي موجودًا.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // إنشاء إعدادات خطوط فردية
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // تعيين بدائل الخط لـ "Arial"
            fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Calibri" });

            try
            {
                // احصل على بدائل الخط لـ "Arial"
                string[] substitutes = fontConfigs.GetFontSubstitutes("Arial");

                Console.WriteLine("Font substitutes for Arial:");
                foreach (string font in substitutes)
                {
                    Console.WriteLine(font);
                }

                // أنشئ دفتر عمل لتوضيح التأثير
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // تعيين نمط باستخدام الخط الأصلي
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "This text uses Arial font which may be substituted";

                // احفظ المصنف
                workbook.Save("FontSubstitutesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontSubstitutes method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



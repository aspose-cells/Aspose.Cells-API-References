---
title: "FontConfigs.SetFontSubstitutes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FontConfigs. أسماء بدائل الخط للخط الأصلي المحدد"
type: docs
url: /ar/net/aspose.cells/fontconfigs/setfontsubstitutes/
---
## FontConfigs.SetFontSubstitutes method

أسماء بدائل الخط للخط الأصلي المحدد.

```csharp
public static void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
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

    public class FontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // اسم الخط الأصلي الذي قد لا يكون متاحًا
            string originalFontName = "Arial";
            
            // أسماء خطوط بديلة للاستخدام عندما لا يكون الأصلي متاحًا
            string[] substituteFontNames = new string[] { "Liberation Sans", "Helvetica", "Verdana" };
            
            try
            {
                // استدعاء طريقة SetFontSubstitutes لتكوين بدائل الخطوط
                FontConfigs.SetFontSubstitutes(originalFontName, substituteFontNames);
                
                Console.WriteLine($"Font substitutes set successfully for '{originalFontName}'");
                
                // تحقق من البدائل عن طريق استرجاعها
                string[] retrievedSubstitutes = FontConfigs.GetFontSubstitutes(originalFontName);
                Console.WriteLine("Current substitutes for '{0}':", originalFontName);
                foreach (string font in retrievedSubstitutes)
                {
                    Console.WriteLine("- " + font);
                }
                
                // تطبيق الخط على خلية لعرض الاستبدال
                worksheet.Cells["A1"].PutValue("Text with potential font substitution");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = originalFontName;
                worksheet.Cells["A1"].SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontSubstitutes method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("FontSubstitutionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



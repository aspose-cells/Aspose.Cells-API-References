---
title: "FontConfigs.GetFontSubstitutes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FontConfigs. تُرجع مصفوفة تحتوي على أسماء بدائل الخط لاستخدامها إذا لم يكن الخط الأصلي موجودًا"
type: docs
url: /ar/net/aspose.cells/fontconfigs/getfontsubstitutes/
---
## FontConfigs.GetFontSubstitutes method

يرجع مصفوفة تحتوي على أسماء بدائل الخطوط التي تُستخدم إذا لم يكن الخط الأصلي موجودًا.

```csharp
public static string[] GetFontSubstitutes(string originalFontName)
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

    public class FontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // تهيئة FontConfigs
            FontConfigs fontConfigs = new FontConfigs();

            try
            {
                // استدعِ GetFontSubstitutes مع اسم الخط
                string originalFontName = "Arial";
                string[] substitutes = FontConfigs.GetFontSubstitutes(originalFontName);

                // عرض النتائج
                Console.WriteLine($"Substitute fonts for '{originalFontName}':");
                if (substitutes != null && substitutes.Length > 0)
                {
                    foreach (string substitute in substitutes)
                    {
                        Console.WriteLine(substitute);
                    }
                }
                else
                {
                    Console.WriteLine("No substitutes found for the specified font.");
                }

                // إظهار تعيين البدائل واسترجاعها
                string[] newSubstitutes = new string[] { "Liberation Sans", "DejaVu Sans" };
                FontConfigs.SetFontSubstitutes(originalFontName, newSubstitutes);

                // احصل على البدائل مرة أخرى للتحقق
                substitutes = FontConfigs.GetFontSubstitutes(originalFontName);
                Console.WriteLine("\nAfter setting substitutes:");
                foreach (string substitute in substitutes)
                {
                    Console.WriteLine(substitute);
                }
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

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "الفئة FontConfigs"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.FontConfigs. تحدد إعدادات الخط"
type: docs
url: /ar/net/aspose.cells/fontconfigs/
---
## FontConfigs class

يحدد إعدادات الخط

```csharp
public class FontConfigs
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [FontConfigs](fontconfigs/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| static [DefaultFontName](../../aspose.cells/fontconfigs/defaultfontname/) { get; set; } | يحصل أو يعيّن اسم الخط الافتراضي. |
| static [PreferSystemFontSubstitutes](../../aspose.cells/fontconfigs/prefersystemfontsubstitutes/) { get; set; } | حدد ما إذا كان يجب استخدام بدائل الخطوط النظامية أولاً أم لا عندما لا يتوفر الخط ولا يتم تعيين بديل لهذا الخط. مثال: على أوبونتو، يتم عادةً استبدال الخط "Arial" بـ "Liberation Sans". القيمة الافتراضية هي false. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [GetFontFileDataInfo](../../aspose.cells/fontconfigs/getfontfiledatainfo/)(string, bool, bool, bool) | احصل على معلومات بيانات ملف الخط. |
| static [GetFontSources](../../aspose.cells/fontconfigs/getfontsources/)() | يحصل على نسخة من المصفوفة التي تحتوي على قائمة المصادر. |
| static [GetFontSubstitutes](../../aspose.cells/fontconfigs/getfontsubstitutes/)(string) | يرجع مصفوفة تحتوي على أسماء بدائل الخطوط التي تُستخدم إذا لم يكن الخط الأصلي موجودًا. |
| static [IsFontAvailable](../../aspose.cells/fontconfigs/isfontavailable/)(string) | حدد ما إذا كان الخط متاحًا. |
| static [SetFontFolder](../../aspose.cells/fontconfigs/setfontfolder/)(string, bool) | يعيّن مجلد الخطوط |
| static [SetFontFolders](../../aspose.cells/fontconfigs/setfontfolders/)(string[], bool) | يعيّن مجلد الخطوط |
| static [SetFontSources](../../aspose.cells/fontconfigs/setfontsources/)(FontSourceBase[]) | يعيّن مصادر الخط. |
| static [SetFontSubstitutes](../../aspose.cells/fontconfigs/setfontsubstitutes/)(string, string[]) | أسماء بدائل الخط للخط الأصلي المحدد. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontConfigsDemo
    {
        public static void Run()
        {
            // تعيين مجلد خطوط مخصص
            string fontFolder = @"C:\MyFonts\";
            FontConfigs.SetFontFolder(fontFolder, true);

            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين نص تجريبي بخطوط مختلفة
            worksheet.Cells["A1"].PutValue("Text with default font");
            worksheet.Cells["A2"].PutValue("Text with custom font");
            
            // تطبيق نمط خط مخصص
            Style style = workbook.CreateStyle();
            style.Font.Name = "MyCustomFont"; // This font should exist in the custom font folder
            worksheet.Cells["A2"].SetStyle(style);

            // احفظ إلى HTML لعرض تجسيد الخط
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportImagesAsBase64 = true,
                PresentationPreference = true
            };
            
            workbook.Save("output.html", options);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



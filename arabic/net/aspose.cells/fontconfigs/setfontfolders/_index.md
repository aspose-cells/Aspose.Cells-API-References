---
title: "FontConfigs.SetFontFolders"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FontConfigs. تحدد مجلد الخطوط"
type: docs
url: /ar/net/aspose.cells/fontconfigs/setfontfolders/
---
## FontConfigs.SetFontFolders method

يعيّن مجلد الخطوط

```csharp
public static void SetFontFolders(string[] fontFolders, bool recursive)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fontFolders | String[] | المجلدات التي تحتوي على خطوط TrueType. |
| recursive | منطقي | يحدد ما إذا كان يجب مسح المجلدات الفرعية أم لا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // حدد بعض النص الذي سيستخدم خطوطًا مخصصة
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // جهّز مجلدات الخطوط (استبدلها بالمسارات الفعلية على نظامك)
            string[] fontFolders = new string[] 
            {
                @"C:\Windows\Fonts",
                @"D:\CustomFonts"
            };
            bool recursiveSearch = true;

            try
            {
                // استدعِ طريقة SetFontFolders مع معلمات String[] و Boolean
                FontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // طبق خطًا قد يكون في أحد هذه المجلدات
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Replace with actual font name
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("Font folders set successfully. Workbook may use fonts from these locations.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font folders: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("FontConfigsSetFontFoldersDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



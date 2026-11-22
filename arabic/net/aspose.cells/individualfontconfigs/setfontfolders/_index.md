---
title: "IndividualFontConfigs.SetFontFolders"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة IndividualFontConfigs. تقوم بتعيين مجلدات الخطوط"
type: docs
url: /ar/net/aspose.cells/individualfontconfigs/setfontfolders/
---
## IndividualFontConfigs.SetFontFolders method

يضبط مجلدات الخطوط

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
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

    public class IndividualFontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نسخة من IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // تحضير مصفوفة مجلدات الخطوط
            string[] fontFolders = new string[] { @"C:\Windows\Fonts", @"D:\CustomFonts" };
            bool recursiveSearch = true;

            try
            {
                // استدعِ طريقة SetFontFolders مع معلمات String[] و Boolean
                fontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // إظهار التأثير باستخدام خط مخصص
                worksheet.Cells["A1"].PutValue("Text with custom font");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Assuming this font exists in one of the folders
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("SetFontFolders method executed successfully with parameters (String[], Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontFolders method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("SetFontFoldersDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



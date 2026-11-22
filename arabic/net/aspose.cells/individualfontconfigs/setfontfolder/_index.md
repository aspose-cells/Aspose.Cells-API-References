---
title: "IndividualFontConfigs.SetFontFolder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة IndividualFontConfigs. تعيين مجلد الخطوط"
type: docs
url: /ar/net/aspose.cells/individualfontconfigs/setfontfolder/
---
## IndividualFontConfigs.SetFontFolder method

يعيّن مجلد الخطوط

```csharp
public void SetFontFolder(string fontFolder, bool recursive)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fontFolder | String | المجلد الذي يحتوي على خطوط TrueType. |
| recursive | منطقي | يحدد ما إذا كان يجب مسح المجلدات الفرعية أم لا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء نسخة من IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();
            
            // حدد مسار مجلد الخطوط وما إذا كان البحث بشكل تكراري
            string fontFolderPath = @"C:\Windows\Fonts";
            bool recursiveSearch = true;

            try
            {
                // استدعِ SetFontFolder مع المعلمات المحددة
                fontConfigs.SetFontFolder(fontFolderPath, recursiveSearch);
                
                Console.WriteLine($"Successfully set font folder to: {fontFolderPath}");
                Console.WriteLine($"Recursive search enabled: {recursiveSearch}");

                // إنشاء مصنف لعرض استخدام الخطوط
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // تعيين نمط قد يستخدم الخطوط من المجلد المحدد
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial"; // Assuming Arial exists in the font folder
                style.Font.Size = 12;
                
                worksheet.Cells["A1"].Value = "Text with font from specified folder";
                worksheet.Cells["A1"].SetStyle(style);
                
                // احفظ المصنف
                workbook.Save("FontConfigDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font folder: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "FontConfigs.GetFontSources"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FontConfigs. تحصل على نسخة من المصفوفة التي تحتوي على قائمة المصادر"
type: docs
url: /ar/net/aspose.cells/fontconfigs/getfontsources/
---
## FontConfigs.GetFontSources method

يحصل على نسخة من المصفوفة التي تحتوي على قائمة المصادر.

```csharp
public static FontSourceBase[] GetFontSources()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodGetFontSourcesDemo
    {
        public static void Run()
        {
            try
            {
                // احصل على مصادر الخط الحالية
                FontSourceBase[] fontSources = FontConfigs.GetFontSources();

                // اعرض معلومات حول كل مصدر خط
                if (fontSources != null)
                {
                    Console.WriteLine("Current font sources:");
                    foreach (var source in fontSources)
                    {
                        Console.WriteLine($"Type: {source.GetType().Name}");
                        if (source is FolderFontSource folderSource)
                        {
                            Console.WriteLine($"Folder path: {folderSource.FolderPath}");
                            Console.WriteLine($"Scan subfolders: {folderSource.ScanSubFolders}");
                        }
                        else if (source is FileFontSource fileSource)
                        {
                            Console.WriteLine($"File path: {fileSource.FilePath}");
                        }
                        else if (source is MemoryFontSource memorySource)
                        {
                            Console.WriteLine($"Font data present: {memorySource.FontData != null}");
                        }
                        Console.WriteLine();
                    }
                }
                else
                {
                    Console.WriteLine("No font sources are currently set.");
                }

                // إنشاء دفتر عمل جديد لعرض التأثير
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // تعيين بعض النص باستخدام خط قد يستخدم هذه المصادر
                worksheet.Cells["A1"].PutValue("Font Sources Demo");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);

                // احفظ المصنف
                workbook.Save("FontConfigsGetFontSourcesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with font sources: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [FontSourceBase](../../fontsourcebase/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



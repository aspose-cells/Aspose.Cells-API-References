---
title: "IndividualFontConfigs.SetFontSources"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة IndividualFontConfigs. تعيين مصادر الخط"
type: docs
url: /ar/net/aspose.cells/individualfontconfigs/setfontsources/
---
## IndividualFontConfigs.SetFontSources method

يعيّن مصادر الخط.

```csharp
public void SetFontSources(FontSourceBase[] sources)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصادر | FontSourceBase[] | مصفوفة من المصادر التي تحتوي على خطوط TrueType. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class IndividualFontConfigsMethodSetFontSourcesWithFontSourceBaseDemo
    {
        public static void Run()
        {
            // إنشاء إعدادات خطوط فردية
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // تحضير مصادر الخط - باستخدام كل من مجلد ومصادر الخط الذاكرة
            FontSourceBase[] fontSources = new FontSourceBase[]
            {
                new FolderFontSource(@"C:\Windows\Fonts", false),
                new MemoryFontSource(File.ReadAllBytes(@"C:\Windows\Fonts\arial.ttf"))
            };

            try
            {
                // استدعاء SetFontSources مع مصادر الخط المُحضرة
                fontConfigs.SetFontSources(fontSources);

                Console.WriteLine("Font sources set successfully:");
                foreach (var source in fontConfigs.GetFontSources())
                {
                    if (source is FolderFontSource folderSource)
                    {
                        Console.WriteLine($"- Folder: {folderSource.FolderPath} (Recursive: {folderSource.ScanSubFolders})");
                    }
                    else if (source is MemoryFontSource memorySource)
                    {
                        Console.WriteLine($"- Memory font with data length: {memorySource.FontData.Length} bytes");
                    }
                }

                // أنشئ دفتر عمل لتوضيح التأثير
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // استخدام خط يجب أن يكون متاحًا من المصادر
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "Text using font from custom sources";
                worksheet.Cells["A2"].Value = "This demonstrates SetFontSources with FontSourceBase[]";

                // احفظ المصنف
                workbook.Save("SetFontSourcesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontSources method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [FontSourceBase](../../fontsourcebase/)
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "FontConfigs.SetFontSources"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FontConfigs. تعيين مصادر الخطوط"
type: docs
url: /ar/net/aspose.cells/fontconfigs/setfontsources/
---
## FontConfigs.SetFontSources method

يعيّن مصادر الخط.

```csharp
public static void SetFontSources(FontSourceBase[] sources)
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

    public class FontConfigsMethodSetFontSourcesWithFontSourceBaseDemo
    {
        public static void Run()
        {
            // أنشئ ملف خط مؤقت للعرض
            string tempFontFile = Path.Combine(Path.GetTempPath(), "testfont.ttf");
            try
            {
                File.WriteAllBytes(tempFontFile, new byte[0]); // Empty file for demo

                // أنشئ مصادر الخطوط
                FontSourceBase[] fontSources = new FontSourceBase[]
                {
                    new FolderFontSource(Path.GetTempPath(), true),
                    new FileFontSource(tempFontFile)
                };

                try
                {
                    // استدعِ طريقة SetFontSources
                    FontConfigs.SetFontSources(fontSources);

                    // تحقق من تعيين مصادر الخطوط
                    FontSourceBase[] currentSources = FontConfigs.GetFontSources();
                    Console.WriteLine($"Font sources set successfully. Count: {currentSources.Length}");

                    // أظهر التأثير عن طريق التحقق مما إذا كان الخط متاحًا
                    bool isAvailable = FontConfigs.IsFontAvailable("Arial");
                    Console.WriteLine($"Is Arial available: {isAvailable}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error executing SetFontSources method: {ex.Message}");
                }
            }
            finally
            {
                // تنظيف
                if (File.Exists(tempFontFile))
                {
                    File.Delete(tempFontFile);
                }
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



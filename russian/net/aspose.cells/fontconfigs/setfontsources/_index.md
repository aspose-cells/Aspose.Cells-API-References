---
title: "FontConfigs.SetFontSources"
second_title: "Справочник API Aspose.Cells для .NET"
description: "FontConfigs method. Устанавливает источники шрифтов"
type: docs
url: /ru/net/aspose.cells/fontconfigs/setfontsources/
---
## FontConfigs.SetFontSources method

Устанавливает источники шрифтов.

```csharp
public static void SetFontSources(FontSourceBase[] sources)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| источники | FontSourceBase[] | Массив источников, содержащих шрифты TrueType. |

### Примеры

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
            // Создайте временный файл шрифта для демонстрации
            string tempFontFile = Path.Combine(Path.GetTempPath(), "testfont.ttf");
            try
            {
                File.WriteAllBytes(tempFontFile, new byte[0]); // Empty file for demo

                // Создайте источники шрифтов
                FontSourceBase[] fontSources = new FontSourceBase[]
                {
                    new FolderFontSource(Path.GetTempPath(), true),
                    new FileFontSource(tempFontFile)
                };

                try
                {
                    // Вызовите метод SetFontSources
                    FontConfigs.SetFontSources(fontSources);

                    // Проверьте, что источники шрифтов были установлены
                    FontSourceBase[] currentSources = FontConfigs.GetFontSources();
                    Console.WriteLine($"Font sources set successfully. Count: {currentSources.Length}");

                    // Продемонстрируйте эффект, проверив, доступен ли шрифт
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
                // Очистить
                if (File.Exists(tempFontFile))
                {
                    File.Delete(tempFontFile);
                }
            }
        }
    }
}
```

### См. также

* class [FontSourceBase](../../fontsourcebase/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



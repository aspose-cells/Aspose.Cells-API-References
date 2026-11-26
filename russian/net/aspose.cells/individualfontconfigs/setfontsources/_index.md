---
title: "IndividualFontConfigs.SetFontSources"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод IndividualFontConfigs. Устанавливает источники шрифтов"
type: docs
url: /ru/net/aspose.cells/individualfontconfigs/setfontsources/
---
## IndividualFontConfigs.SetFontSources method

Устанавливает источники шрифтов.

```csharp
public void SetFontSources(FontSourceBase[] sources)
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

    public class IndividualFontConfigsMethodSetFontSourcesWithFontSourceBaseDemo
    {
        public static void Run()
        {
            // Создать индивидуальные конфигурации шрифтов
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Подготовить источники шрифтов — использовать как папочный, так и памятьный источники шрифтов
            FontSourceBase[] fontSources = new FontSourceBase[]
            {
                new FolderFontSource(@"C:\Windows\Fonts", false),
                new MemoryFontSource(File.ReadAllBytes(@"C:\Windows\Fonts\arial.ttf"))
            };

            try
            {
                // Вызвать SetFontSources с подготовленными источниками шрифтов
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

                // Создать книгу для демонстрации эффекта
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Использовать шрифт, который должен быть доступен из источников
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "Text using font from custom sources";
                worksheet.Cells["A2"].Value = "This demonstrates SetFontSources with FontSourceBase[]";

                // Сохраните книгу
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

### См. также

* class [FontSourceBase](../../fontsourcebase/)
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



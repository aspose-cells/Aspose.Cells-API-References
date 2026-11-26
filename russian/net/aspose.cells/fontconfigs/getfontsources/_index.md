---
title: "FontConfigs.GetFontSources"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FontConfigs. Возвращает копию массива, содержащего список источников"
type: docs
url: /ru/net/aspose.cells/fontconfigs/getfontsources/
---
## FontConfigs.GetFontSources method

Получает копию массива, содержащего список источников

```csharp
public static FontSourceBase[] GetFontSources()
```

### Примеры

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
                // Получите текущие источники шрифтов
                FontSourceBase[] fontSources = FontConfigs.GetFontSources();

                // Отобразите информацию о каждом источнике шрифтов
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

                // Создайте новую книгу для демонстрации эффекта
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Установите некоторый текст шрифтом, который может использовать эти источники
                worksheet.Cells["A1"].PutValue("Font Sources Demo");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);

                // Сохраните книгу
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

### См. также

* class [FontSourceBase](../../fontsourcebase/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



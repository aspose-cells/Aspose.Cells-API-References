---
title: "IndividualFontConfigs.GetFontSources"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод IndividualFontConfigs. Возвращает копию массива, содержащего список источников"
type: docs
url: /ru/net/aspose.cells/individualfontconfigs/getfontsources/
---
## IndividualFontConfigs.GetFontSources method

Получает копию массива, содержащего список источников

```csharp
public FontSourceBase[] GetFontSources()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSourcesDemo
    {
        public static void Run()
        {
            // Создать индивидуальные конфигурации шрифтов
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Установить некоторые источники шрифтов (папки, содержащие шрифты)
            string fontFolder1 = @"C:\Windows\Fonts";
            string fontFolder2 = @"D:\CustomFonts";
            fontConfigs.SetFontFolder(fontFolder1, false);
            fontConfigs.SetFontFolder(fontFolder2, true);

            try
            {
                // Получите текущие источники шрифтов
                FontSourceBase[] fontSources = fontConfigs.GetFontSources();

                Console.WriteLine("Current font sources:");
                foreach (var source in fontSources)
                {
                    if (source is FolderFontSource folderSource)
                    {
                        Console.WriteLine($"- Folder: {folderSource.FolderPath} (Recursive: {folderSource.ScanSubFolders})");
                    }
                }

                // Создать книгу для демонстрации эффекта
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                // Использовать конфигурации шрифтов при создании стилей или работе с шрифтами
                // (У Workbook нет свойства FontConfigs, поэтому мы удаляем эту строку)
                Worksheet worksheet = workbook.Worksheets[0];

                // Использовать пользовательский шрифт, который может находиться в одной из папок
                Style style = workbook.CreateStyle();
                style.Font.Name = "SomeCustomFont";
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text with custom font");

                Console.WriteLine("Workbook created with custom font configurations.");
                workbook.Save("MethodGetFontSourcesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontSources method: {ex.Message}");
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



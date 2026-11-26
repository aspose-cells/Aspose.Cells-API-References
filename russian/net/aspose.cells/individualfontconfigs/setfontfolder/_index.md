---
title: "IndividualFontConfigs.SetFontFolder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод IndividualFontConfigs. Устанавливает папку шрифтов"
type: docs
url: /ru/net/aspose.cells/individualfontconfigs/setfontfolder/
---
## IndividualFontConfigs.SetFontFolder method

Устанавливает папку шрифтов

```csharp
public void SetFontFolder(string fontFolder, bool recursive)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fontFolder | String | Папка, содержащая TrueType‑шрифты. |
| recursive | Boolean | Определяет, следует ли сканировать подпапки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // Создать экземпляр IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();
            
            // Указать путь к папке шрифтов и нужно ли выполнять рекурсивный поиск
            string fontFolderPath = @"C:\Windows\Fonts";
            bool recursiveSearch = true;

            try
            {
                // Вызвать SetFontFolder с указанными параметрами
                fontConfigs.SetFontFolder(fontFolderPath, recursiveSearch);
                
                Console.WriteLine($"Successfully set font folder to: {fontFolderPath}");
                Console.WriteLine($"Recursive search enabled: {recursiveSearch}");

                // Создать книгу для демонстрации использования шрифтов
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Установить стиль, который может использовать шрифты из указанной папки
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial"; // Assuming Arial exists in the font folder
                style.Font.Size = 12;
                
                worksheet.Cells["A1"].Value = "Text with font from specified folder";
                worksheet.Cells["A1"].SetStyle(style);
                
                // Сохраните книгу
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

### См. также

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



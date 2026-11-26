---
title: "FontConfigs.SetFontFolders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FontConfigs. Устанавливает папку шрифтов"
type: docs
url: /ru/net/aspose.cells/fontconfigs/setfontfolders/
---
## FontConfigs.SetFontFolders method

Устанавливает папку шрифтов

```csharp
public static void SetFontFolders(string[] fontFolders, bool recursive)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fontFolders | String[] | Папки, содержащие TrueType‑шрифты. |
| recursive | Boolean | Определяет, следует ли сканировать подпапки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите некоторый текст, который будет использовать пользовательские шрифты
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // Подготовьте папки шрифтов (замените их фактическими путями в вашей системе)
            string[] fontFolders = new string[] 
            {
                @"C:\Windows\Fonts",
                @"D:\CustomFonts"
            };
            bool recursiveSearch = true;

            try
            {
                // Вызовите метод SetFontFolders с параметрами String[] и Boolean
                FontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // Примените шрифт, который может находиться в одной из этих папок
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Replace with actual font name
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("Font folders set successfully. Workbook may use fonts from these locations.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font folders: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("FontConfigsSetFontFoldersDemo.xlsx");
        }
    }
}
```

### См. также

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



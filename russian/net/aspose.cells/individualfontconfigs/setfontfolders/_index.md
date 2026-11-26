---
title: "IndividualFontConfigs.SetFontFolders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод IndividualFontConfigs. Устанавливает папки шрифтов"
type: docs
url: /ru/net/aspose.cells/individualfontconfigs/setfontfolders/
---
## IndividualFontConfigs.SetFontFolders method

Устанавливает папки шрифтов

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
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

    public class IndividualFontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать экземпляр IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Подготовить массив папок шрифтов
            string[] fontFolders = new string[] { @"C:\Windows\Fonts", @"D:\CustomFonts" };
            bool recursiveSearch = true;

            try
            {
                // Вызовите метод SetFontFolders с параметрами String[] и Boolean
                fontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // Продемонстрировать эффект, используя пользовательский шрифт
                worksheet.Cells["A1"].PutValue("Text with custom font");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Assuming this font exists in one of the folders
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("SetFontFolders method executed successfully with parameters (String[], Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontFolders method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("SetFontFoldersDemo.xlsx");
        }
    }
}
```

### См. также

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



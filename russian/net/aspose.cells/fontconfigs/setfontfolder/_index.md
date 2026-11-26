---
title: "FontConfigs.SetFontFolder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FontConfigs. Устанавливает папку шрифтов"
type: docs
url: /ru/net/aspose.cells/fontconfigs/setfontfolder/
---
## FontConfigs.SetFontFolder method

Устанавливает папку шрифтов

```csharp
public static void SetFontFolder(string fontFolder, bool recursive)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fontFolder | String | Папка, содержащая TrueType‑шрифты. |
| recursive | Boolean | Определяет, следует ли сканировать подпапки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // Инициализировать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторый текст в ячейку A1
            worksheet.Cells["A1"].PutValue("Sample Text with Custom Font");
            
            // Установите пользовательскую папку шрифтов и укажите, включать ли подпапки
            FontConfigs.SetFontFolder("Fonts", true);
            
            // Примените стиль шрифта, который может использовать шрифты из пользовательской папки
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "CustomFont"; // Assuming "CustomFont" exists in the Fonts folder
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Сохраните книгу в PDF
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### См. также

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



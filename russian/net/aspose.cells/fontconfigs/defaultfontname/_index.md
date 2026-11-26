---
title: "FontConfigs.DefaultFontName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FontConfigs. Получает или задает имя шрифта по умолчанию"
type: docs
url: /ru/net/aspose.cells/fontconfigs/defaultfontname/
---
## FontConfigs.DefaultFontName property

Получает или задает имя шрифта по умолчанию.

```csharp
public static string DefaultFontName { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyDefaultFontNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Отобразить текущее имя шрифта по умолчанию
            Console.WriteLine("Current DefaultFontName value: " + FontConfigs.DefaultFontName);

            // Установить новое имя шрифта по умолчанию
            FontConfigs.DefaultFontName = "Arial";

            // Создать стиль без явно заданного шрифта, чтобы продемонстрировать использование шрифта по умолчанию
            Style style = workbook.CreateStyle();
            style.Font.Name = ""; // Empty to use default font

            // Применить стиль к ячейке
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text should use the default font");
            cell.SetStyle(style);

            // Сохранить рабочую книгу, чтобы увидеть эффект
            workbook.Save("PropertyDefaultFontNameDemo.xlsx");

            // Проверить, что шрифт был применён корректно
            Console.WriteLine("Cell font after setting DefaultFontName: " + cell.GetStyle().Font.Name);
        }
    }
}
```

### См. также

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



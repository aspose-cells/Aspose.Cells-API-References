---
title: "TextOptions.LanguageCode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextOptions. Получает и задает язык пользовательского интерфейса"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textoptions/languagecode/
---
## TextOptions.LanguageCode property

Получает и задает язык пользовательского интерфейса.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте фигуру и задайте её текст
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample text with language settings";

            // Установите код языка для параметров текста фигуры
            shape.TextOptions.LanguageCode = CountryCode.Japan;

            // Проверьте и выведите код языка
            Console.WriteLine("Shape Text Language Code: " + shape.TextOptions.LanguageCode);

            // Сохраните книгу
            workbook.Save("TextOptionsLanguageDemo.xlsx");
        }
    }
}
```

### См. также

* enum [CountryCode](../../../aspose.cells/countrycode/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



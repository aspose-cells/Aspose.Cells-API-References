---
title: "HtmlSaveOptions.DefaultFontName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает имя шрифта по умолчанию для экспорта html; шрифт по умолчанию будет использоваться, когда шрифт стиля отсутствует. Если это свойство равно null, Aspose.Cells будет использовать универсальный шрифт, имеющий ту же семейство, что и оригинальный шрифт. Значение по умолчанию — null."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/defaultfontname/
---
## HtmlSaveOptions.DefaultFontName property

Укажите имя шрифта по умолчанию для экспорта HTML; этот шрифт будет использоваться, если шрифт стиля отсутствует. Если это свойство равно null, Aspose.Cells использует универсальный шрифт той же семейства, что и оригинальный шрифт. Значение по умолчанию — null.

```csharp
public string DefaultFontName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyDefaultFontNameDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // Установите параметры сохранения HTML с пользовательским шрифтом по умолчанию
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.DefaultFontName = "Courier New";
            
            // Сохраните в HTML с указанным шрифтом
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with default font: " + saveOptions.DefaultFontName);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



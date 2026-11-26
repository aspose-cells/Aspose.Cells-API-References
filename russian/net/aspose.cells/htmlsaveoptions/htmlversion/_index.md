---
title: "HtmlSaveOptions.HtmlVersion"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает версию стандарта HTML, которая должна использоваться при сохранении в формате HTML. Значение по умолчанию — HtmlVersion.Default"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/htmlversion/
---
## HtmlSaveOptions.HtmlVersion property

Указывает версию стандарта HTML, которая должна использоваться при сохранении в формате HTML. Значение по умолчанию — HtmlVersion.Default.

```csharp
public HtmlVersion HtmlVersion { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyHtmlVersionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion property");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["C4"].PutValue("Sample Text");
            
            // Создать экземпляр HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Отобразить текущее значение HtmlVersion
            Console.WriteLine("Current HtmlVersion: " + options.HtmlVersion);
            
            // Установить HtmlVersion в HTML5
            options.HtmlVersion = HtmlVersion.Html5;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // Сохранить с версией HTML5
            workbook.Save("HtmlVersion_Html5.html", options);
            
            // Переключить на XHTML
            options.HtmlVersion = HtmlVersion.XHtml;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // Сохранить с версией XHTML
            workbook.Save("HtmlVersion_XHtml.html", options);
            
            // Сбросить к значению по умолчанию
            options.HtmlVersion = HtmlVersion.Default;
            Console.WriteLine("HtmlVersion reset to: " + options.HtmlVersion);
            
            // Сохранить с версией по умолчанию
            workbook.Save("HtmlVersion_Default.html", options);
        }
    }
}
```

### См. также

* enum [HtmlVersion](../../htmlversion/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



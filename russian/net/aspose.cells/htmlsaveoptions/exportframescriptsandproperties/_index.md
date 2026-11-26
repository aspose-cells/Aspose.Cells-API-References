---
title: "HtmlSaveOptions.ExportFrameScriptsAndProperties"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли скрипты кадров и свойства документа. Значение по умолчанию — true. Если вы хотите импортировать html или mht файл в Excel, пожалуйста, оставьте значение по умолчанию"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportframescriptsandproperties/
---
## HtmlSaveOptions.ExportFrameScriptsAndProperties property

Указывает, экспортировать ли скрипты фрейма и свойства документа. Значение по умолчанию — true.If вы хотите импортировать файл html или mht в Excel, пожалуйста, оставьте значение по умолчанию.

```csharp
public bool ExportFrameScriptsAndProperties { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportFrameScriptsAndPropertiesDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Установить параметры сохранения HTML с ExportFrameScriptsAndProperties
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportFrameScriptsAndProperties = true;

            // Сохранить как HTML
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with ExportFrameScriptsAndProperties enabled.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "HtmlSaveOptions.EncodeEntityAsCode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, заменяются ли HTML‑символьные сущности десятичным кодом. Например, nbsp заменяется на 160. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/encodeentityascode/
---
## HtmlSaveOptions.EncodeEntityAsCode property

Указывает, заменяются ли HTML‑символьные сущности на десятичные коды. (например, \"&amp;nbsp;\" заменяется на \"&amp;#160;\"). Значение по умолчанию — false.

```csharp
public bool EncodeEntityAsCode { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class HtmlSaveOptionsPropertyEncodeEntityAsCodeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные со специальными символами
            worksheet.Cells["A1"].PutValue("Sample & Text");
            worksheet.Cells["A2"].PutValue("Another <Test> String");
            worksheet.Cells["A3"].PutValue("Price: $100");

            // Создать параметры сохранения HTML
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Отобразите текущее значение EncodeEntityAsCode
            Console.WriteLine("Current EncodeEntityAsCode value: " + options.EncodeEntityAsCode);

            // Установите EncodeEntityAsCode в true
            options.EncodeEntityAsCode = true;

            // Сохраните с кодированными сущностями в виде кода
            workbook.Save("HtmlWithEncodedEntities.html", options);

            // Установите EncodeEntityAsCode в false
            options.EncodeEntityAsCode = false;

            // Сохраните сущности без изменений
            workbook.Save("HtmlWithRawEntities.html", options);

            // Сравните выходные файлы
            Console.WriteLine("Files created:");
            Console.WriteLine("1. HtmlWithEncodedEntities.html - with encoded entities");
            Console.WriteLine("2. HtmlWithRawEntities.html - with raw entities");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



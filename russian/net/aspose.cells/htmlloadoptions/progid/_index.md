---
title: "HtmlLoadOptions.ProgId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlLoadOptions. Получает идентификатор программы, создающей файл. Только для файлов MHT"
type: docs
url: /ru/net/aspose.cells/htmlloadoptions/progid/
---
## HtmlLoadOptions.ProgId property

Получает идентификатор программы, создавшей файл. Только для файлов MHT.

```csharp
public string ProgId { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyProgIdDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки HTML в формате MHTML
            HtmlLoadOptions options = new HtmlLoadOptions(LoadFormat.MHtml);
            
            // Получить свойство ProgId
            Console.WriteLine("ProgId is: " + options.ProgId);

            // Создать другой экземпляр и получить его ProgId
            HtmlLoadOptions wordOptions = new HtmlLoadOptions(LoadFormat.MHtml);
            Console.WriteLine("ProgId is: " + wordOptions.ProgId);
        }
    }
}
```

### См. также

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



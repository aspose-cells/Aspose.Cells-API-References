---
title: "DocumentProperty.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DocumentProperty. Получает или задает значение свойства"
type: docs
url: /ru/net/aspose.cells.properties/documentproperty/value/
---
## DocumentProperty.Value property

Получает или задает значение свойства.

```csharp
public object Value { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к встроенным свойствам документа
            var hyperlinkBase = workbook.Worksheets.BuiltInDocumentProperties["HyperlinkBase"];
            hyperlinkBase.Value = "http://www.example.com";

            var title = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            title.Value = "Sample Document Title";

            // Сохраните книгу
            workbook.Save("DocumentPropertiesDemo.xlsx");

            // Отобразите установленные значения
            Console.WriteLine("HyperlinkBase: " + hyperlinkBase.Value);
            Console.WriteLine("Title: " + title.Value);
        }
    }
}
```

### См. также

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



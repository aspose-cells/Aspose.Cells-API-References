---
title: "XmlSaveOptions.HasHeaderRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XmlSaveOptions. Указывает, содержит ли диапазон строку заголовка"
type: docs
url: /ru/net/aspose.cells/xmlsaveoptions/hasheaderrow/
---
## XmlSaveOptions.HasHeaderRow property

Указывает, содержит ли диапазон строку заголовка.

```csharp
public bool HasHeaderRow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте строку заголовка и данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создайте параметры сохранения XML
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.HasHeaderRow = true; // Demonstrate HasHeaderRow property
            saveOptions.SheetNameAsElementName = true;

            // Сохранить как файл XML
            workbook.Save("output.xml", saveOptions);

            Console.WriteLine("XML file saved with HasHeaderRow=true");
        }
    }
}
```

### См. также

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



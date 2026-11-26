---
title: "XmlLoadOptions.IgnoreRootAttributes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XmlLoadOptions. Указывает, игнорировать ли атрибуты корневого элемента"
type: docs
url: /ru/net/aspose.cells/xmlloadoptions/ignorerootattributes/
---
## XmlLoadOptions.IgnoreRootAttributes property

Указывает, следует ли игнорировать атрибуты корневого элемента.

```csharp
public bool IgnoreRootAttributes { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIgnoreRootAttributesDemo
    {
        public static void Run()
        {
            // Создайте параметры загрузки XML и установите IgnoreRootAttributes
            XmlLoadOptions options = new XmlLoadOptions();
            options.IgnoreRootAttributes = true;

            // Загрузите файл XML с этими параметрами
            Workbook workbook = new Workbook("example.xml", options);

            // Получите доступ к данным из загруженного XML
            string cellValue = workbook.Worksheets[0].Cells["AH8"].StringValue;
            Console.WriteLine("Cell AH8 value: " + cellValue);

            // Сохранить как XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



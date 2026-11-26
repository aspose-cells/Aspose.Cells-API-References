---
title: "XmlLoadOptions.DateFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XmlLoadOptions. Получает и задает формат значения даты"
type: docs
url: /ru/net/aspose.cells/xmlloadoptions/dateformat/
---
## XmlLoadOptions.DateFormat property

Получает и задает формат значения даты.

```csharp
public string DateFormat { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Создайте экземпляр XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Установите формат даты для разбора дат из XML
            options.DateFormat = "yyyy-MM-dd";
            options.ConvertNumericOrDate = true;

            // Загрузите XML‑файл в Workbook, используя указанные параметры
            Workbook workbook = new Workbook("input.xml", options);

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Отобразите некоторые ячейки, чтобы продемонстрировать форматирование дат
            Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].Value);

            // Сохраните книгу в новый файл
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



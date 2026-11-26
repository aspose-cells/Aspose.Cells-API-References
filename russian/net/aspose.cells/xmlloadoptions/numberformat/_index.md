---
title: "XmlLoadOptions.NumberFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XmlLoadOptions. Получает и задает формат числового значения"
type: docs
url: /ru/net/aspose.cells/xmlloadoptions/numberformat/
---
## XmlLoadOptions.NumberFormat property

Получает и задает формат числового значения.

```csharp
public string NumberFormat { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Создайте экземпляр XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Установите свойство NumberFormat, чтобы отображать числа с 2 знаками после запятой
            options.NumberFormat = "0.00";

            // Загрузите XML‑файл в Workbook, используя указанные параметры
            Workbook workbook = new Workbook("input.xml", options);

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите некоторые числовые значения, чтобы продемонстрировать форматирование чисел
            worksheet.Cells["A1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(45.678);
            worksheet.Cells["A3"].PutValue(0.5);

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



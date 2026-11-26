---
title: "AbstractTextLoadOptions.KeepPrecision"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AbstractTextLoadOptions. Указывает, не разбирать строковое значение, если его длина равна 15"
type: docs
url: /ru/net/aspose.cells/abstracttextloadoptions/keepprecision/
---
## AbstractTextLoadOptions.KeepPrecision property

Указывает, не разбирать строковое значение, если его длина равна 15.

```csharp
public bool KeepPrecision { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyKeepPrecisionDemo
    {
        public static void Run()
        {
            // Создайте параметры загрузки HTML и установите KeepPrecision в true
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.KeepPrecision = true;

            // Загрузите книгу с параметрами
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Продемонстрируйте сохранение точности (например, числовые значения с большим количеством знаков после запятой)
            Cell cell = worksheet.Cells["A1"];
            Console.WriteLine("Value with precision: " + cell.Value);

            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



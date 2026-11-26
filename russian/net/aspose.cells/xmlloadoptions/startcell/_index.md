---
title: "XmlLoadOptions.StartCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XmlLoadOptions. Получает и задает начальную ячейку"
type: docs
url: /ru/net/aspose.cells/xmlloadoptions/startcell/
---
## XmlLoadOptions.StartCell property

Получает и задает начальную ячейку.

```csharp
public string StartCell { get; set; }
```

### Примечания

Работает только когда файл не является speadsheetML или не выполняется сопоставление XML с Excel.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // Создайте экземпляр XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Установите начальную ячейку для импорта данных XML
            options.StartCell = "B2";

            // Загрузите XML‑файл в Workbook, используя указанные параметры
            Workbook workbook = new Workbook("input.xml", options);

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Выведите значение из начальной ячейки, чтобы продемонстрировать свойство
            Console.WriteLine("Value at start cell (B2): " + worksheet.Cells["B2"].Value);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



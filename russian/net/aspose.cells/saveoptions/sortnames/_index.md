---
title: "SaveOptions.SortNames"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SaveOptions. Указывает, следует ли сортировать определённые имена перед сохранением файла"
type: docs
url: /ru/net/aspose.cells/saveoptions/sortnames/
---
## SaveOptions.SortNames property

Указывает, следует ли сортировать определённые имена перед сохранением файла.

```csharp
public bool SortNames { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertySortNamesDemo
    {
        public static void Run()
        {
            // Создайте новый объект Workbook
            Workbook workbook = new Workbook();
            
            // Добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Создать именованный диапазон
            worksheet.Cells.CreateRange("A2:B3").Name = "MyDataRange";

            // Создайте параметры сохранения с включённым SortNames
            XlsSaveOptions saveOptions = new XlsSaveOptions
            {
                SortNames = true
            };

            // Сохраните книгу
            workbook.Save("SortedNamesExample.xls", saveOptions);

            Console.WriteLine("Workbook saved with sorted named ranges.");
        }
    }
}
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



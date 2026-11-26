---
title: "FindOptions.LookInType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FindOptions. Тип поиска"
type: docs
url: /ru/net/aspose.cells/findoptions/lookintype/
---
## FindOptions.LookInType property

Посмотреть в типе.

```csharp
public LookInType LookInType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookInTypeDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу и добавьте примерные данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить значения и формулы в ячейках
            worksheet.Cells["A1"].PutValue("SearchValue");
            worksheet.Cells["A2"].Formula = "=A1";
            worksheet.Cells["B1"].PutValue("OtherValue");

            // Создать параметры поиска для поиска только в формулах
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            // Искать значение в формулах
            Cell foundCell = worksheet.Cells.Find("SearchValue", null, options);

            // Вывести результат.
            if (foundCell != null)
            {
                Console.WriteLine($"Found at: Row {foundCell.Row}, Column {foundCell.Column}");
            }
            else
            {
                Console.WriteLine("Value not found in formulas");
            }
        }
    }
}
```

### См. также

* enum [LookInType](../../lookintype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



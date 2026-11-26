---
title: "Cell.GetValidation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получает проверку, применённую к этой ячейке"
type: docs
url: /ru/net/aspose.cells/cell/getvalidation/
---
## Cell.GetValidation method

Получает проверку, применённую к этой ячейке.

```csharp
public Validation GetValidation()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetValidationDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получите доступ к ячейке B5 и добавьте проверку
            Cell cell = worksheet.Cells["B5"];
            Validation validation = cell.GetValidation();
            
            // Установите тип проверки и покажите сообщение
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            validation.ShowError = true;
            validation.ErrorMessage = "Enter value between 10 and 20";
            
            // Сохраните книгу
            workbook.Save("ValidationDemo.xlsx");
            
            // Проверьте проверку
            Validation retrievedValidation = cell.GetValidation();
            Console.WriteLine("Validation Type: " + retrievedValidation.Type);
            Console.WriteLine("Validation Message: " + retrievedValidation.ErrorMessage);
        }
    }
}
```

### См. также

* class [Validation](../../validation/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



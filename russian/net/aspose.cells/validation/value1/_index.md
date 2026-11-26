---
title: "Validation.Value1"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Validation. Представляет первое значение, связанное с проверкой данных"
type: docs
url: /ru/net/aspose.cells/validation/value1/
---
## Validation.Value1 property

Представляет первое значение, связанное с проверкой данных.

```csharp
public object Value1 { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyValue1Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте проверку в ячейке A1
            Validation validation = worksheet.Cells["A1"].GetValidation();
            validation.Type = ValidationType.List;
            
            // Установите свойство Value1 с массивом строк
            validation.Value1 = new object[] { "Option1", "Option2", "Option3" };

            // Получите и отобразите значения проверки
            object[] values = validation.Value1 as object[];
            Console.WriteLine("Validation values in A1:");
            foreach (object value in values)
            {
                Console.WriteLine(value.ToString());
            }

            // Создайте ещё одну проверку в ячейке B1 с другими значениями
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Value1 = new object[] { "Yes", "No", "Maybe" };

            // Получите и отобразите значения второй проверки
            object[] values2 = validation2.Value1 as object[];
            Console.WriteLine("\nValidation values in B1:");
            foreach (object value in values2)
            {
                Console.WriteLine(value.ToString());
            }
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



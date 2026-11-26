---
title: "Validation.Formula2"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Validation. Представляет значение или выражение, связанное с проверкой данных"
type: docs
url: /ru/net/aspose.cells/validation/formula2/
---
## Validation.Formula2 property

Представляет значение или выражение, связанное с проверкой данных.

```csharp
public string Formula2 { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyFormula2Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            sheet.Cells["B3"].PutValue(100);
            sheet.Cells["B7"].PutValue(50);
            
            // Создать проверку для ячейки B7
            Validation validation = sheet.Cells["B7"].GetValidation();
            
            // Установить тип проверки и формулы
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "=B3";  // Demonstrating Formula2 usage
            
            // Применить проверку
            CellArea area = new CellArea();
            area.StartRow = 6;
            area.StartColumn = 1;
            area.EndRow = 6;
            area.EndColumn = 1;
            validation.AddArea(area);
            
            // Сохраните книгу
            workbook.Save("ValidationFormula2Demo.xlsx");
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



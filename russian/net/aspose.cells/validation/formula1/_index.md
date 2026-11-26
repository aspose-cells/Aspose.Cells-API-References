---
title: "Validation.Formula1"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Validation. Представляет значение или выражение, связанное с проверкой данных"
type: docs
url: /ru/net/aspose.cells/validation/formula1/
---
## Validation.Formula1 property

Представляет значение или выражение, связанное с проверкой данных.

```csharp
public string Formula1 { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyFormula1Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить проверку списка с Formula1 в виде значений, разделённых запятыми
            Validation validation1 = worksheet.Validations[worksheet.Validations.Add()];
            validation1.Type = ValidationType.List;
            validation1.AlertStyle = ValidationAlertType.Stop;
            validation1.Formula1 = "A,B,C";
            validation1.AddArea(new CellArea() { StartRow = 0, StartColumn = 0, EndRow = 5, EndColumn = 0 });

            // Добавить проверку формулы с Formula1 в виде ссылки на ячейку
            Validation validation2 = worksheet.Validations[worksheet.Validations.Add()];
            validation2.Type = ValidationType.Custom;
            validation2.AlertStyle = ValidationAlertType.Stop;
            validation2.Formula1 = "=A5";
            validation2.AddArea(new CellArea() { StartRow = 0, StartColumn = 1, EndRow = 5, EndColumn = 1 });

            // Сохранить и перезагрузить, чтобы проверить сохранность
            string outputPath = "output_validation_formula1.xlsx";
            workbook.Save(outputPath);

            // Перезагрузить для проверки
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];

            Console.WriteLine("Validation 1 Formula1: " + loadedSheet.Validations[0].Formula1);
            Console.WriteLine("Validation 2 Formula1: " + loadedSheet.Validations[1].Formula1);
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



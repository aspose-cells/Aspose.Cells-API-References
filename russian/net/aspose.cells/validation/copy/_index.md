---
title: "Validation.Copy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Validation. Копировать проверку"
type: docs
url: /ru/net/aspose.cells/validation/copy/
---
## Validation.Copy method

Копировать проверку.

```csharp
public void Copy(Validation source, CopyOptions copyOption)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| источник | Проверка | Проверка источника. |
| copyOption | CopyOptions | Опция копирования. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodCopyWithValidationCopyOptionsDemo
    {
        public static void Run()
        {
            // Создать исходную книгу с образцами данных и проверкой
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Добавить образец проверки на исходный лист
            Validation sourceValidation = sourceSheet.Validations[sourceSheet.Validations.Add()];
            sourceValidation.Type = ValidationType.WholeNumber;
            sourceValidation.Operator = OperatorType.Between;
            sourceValidation.Formula1 = "10";
            sourceValidation.Formula2 = "20";
            
            // Создать CellArea с параметрами StartRow, StartColumn, EndRow, EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            sourceValidation.AddArea(area);

            // Создайте целевую книгу
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Добавить проверку на лист назначения (будет перезаписана при копировании)
            Validation destValidation = destSheet.Validations[destSheet.Validations.Add()];
            destValidation.AddArea(area); // Reuse the same area definition

            // Продемонстрировать метод Copy с CopyOptions
            CopyOptions options = new CopyOptions();
            destValidation.Copy(sourceValidation, options);

            // Проверить, что проверка была скопирована корректно
            Console.WriteLine("Validation Type: " + destValidation.Type);
            Console.WriteLine("Validation Formula1: " + destValidation.Formula1);
            Console.WriteLine("Validation Formula2: " + destValidation.Formula2);
        }
    }
}
```

### См. также

* class [CopyOptions](../../copyoptions/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



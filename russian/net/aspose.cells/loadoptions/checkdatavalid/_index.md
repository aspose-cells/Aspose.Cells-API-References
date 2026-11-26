---
title: "LoadOptions.CheckDataValid"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Проверяет, действительны ли данные в файле шаблона"
type: docs
url: /ru/net/aspose.cells/loadoptions/checkdatavalid/
---
## LoadOptions.CheckDataValid property

Проверьте, действительны ли данные в шаблонном файле.

```csharp
public bool CheckDataValid { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCheckDataValidDemo
    {
        public static void Run()
        {
            // Создайте параметры загрузки с CheckDataValid, установленным в false
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            options.CheckDataValid = false;

            // Загрузите книгу с этими параметрами
            Workbook workbook = new Workbook("example.xlsx", options);

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторую проверку данных для демонстрации
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "100";

            // Установить диапазон проверки
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 10;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



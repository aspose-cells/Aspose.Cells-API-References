---
title: "NumbersLoadOptions.LoadTableType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство NumbersLoadOptions. Получает и задает тип загрузки нескольких таблиц в одном листе"
type: docs
url: /ru/net/aspose.cells.numbers/numbersloadoptions/loadtabletype/
---
## NumbersLoadOptions.LoadTableType property

Получает и задает тип загрузки нескольких таблиц в одном листе.

```csharp
public LoadNumbersTableType LoadTableType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsPropertyLoadTableTypeDemo
    {
        public static void Run()
        {
            // Создать экземпляр NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Продемонстрировать использование свойства LoadTableType
                LoadTableType = LoadNumbersTableType.OneTablePerSheet,
                
                // Другие минимально необходимые свойства
                Password = "password123",
                ParsingFormulaOnOpen = true
            };

            // Загрузить файл Numbers с указанными параметрами загрузки
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // Сохранить книгу в формате XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* enum [LoadNumbersTableType](../../loadnumberstabletype/)
* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)



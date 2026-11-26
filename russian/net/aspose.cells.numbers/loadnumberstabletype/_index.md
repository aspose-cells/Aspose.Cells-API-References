---
title: "Перечисление LoadNumbersTableType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Numbers.LoadNumbersTableType enum. Указывает тип загрузки таблиц, когда некоторые таблицы находятся на листе"
type: docs
url: /ru/net/aspose.cells.numbers/loadnumberstabletype/
---
## LoadNumbersTableType enumeration

Указывает тип загрузки таблиц, когда некоторые таблицы находятся в листе.

```csharp
public enum LoadNumbersTableType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| OneTablePerSheet | `1` |  |
| OverrideOtherTables | `2` |  |
| TileTables | `4` |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Numbers;
    using System;

    public class LoadNumbersTableTypeDemo
    {
        public static void LoadNumbersTableTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создать новый лист
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать экземпляр NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions();

            // Установить свойство LoadNumbersTableType
            loadOptions.LoadTableType = LoadNumbersTableType.OneTablePerSheet;

            // Загрузить файл Numbers с указанными параметрами загрузки
            workbook = new Workbook("LoadNumbersTableTypeExample_original.numbers", loadOptions);

            // Сохраните Workbook в файл Excel
            workbook.Save("LoadNumbersTableTypeExample.xlsx");

            Console.WriteLine("Workbook loaded and saved successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Numbers](../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../)



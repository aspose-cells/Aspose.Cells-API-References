---
title: "Перечисление TxtLoadStyleStrategy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.TxtLoadStyleStrategy. Указывает, как применять стиль к разобранным значениям при преобразовании строкового значения в число или дату/время"
type: docs
url: /ru/net/aspose.cells/txtloadstylestrategy/
---
## TxtLoadStyleStrategy enumeration

Указывает, как применять стиль к разобранным значениям при преобразовании строкового значения в число или дату/время.

```csharp
public enum TxtLoadStyleStrategy
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Не задаёт стиль для разобранного значения. |
| BuiltIn | `1` | Устанавливает стиль как встроенный номер/дата‑время, когда разобранное значение является простым числовым/датовым значением. |
| ExactFormat | `2` | Устанавливает точный пользовательский формат для разобранного значения, чтобы отформатированное значение совпадало с исходным вводом. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtLoadStyleStrategyDemo
    {
        public static void TxtLoadStyleStrategyExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Определите пример содержимого CSV
            string csvContent = "Name,Date,Value\nJohn,2023-01-01,100\nDoe,2023-01-02,200";

            // Сохраните содержимое CSV во временный файл
            string tempCsvFilePath = "sample.csv";
            System.IO.File.WriteAllText(tempCsvFilePath, csvContent);

            // Создайте TxtLoadOptions и задайте LoadStyleStrategy
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.LoadStyleStrategy = TxtLoadStyleStrategy.ExactFormat;

            // Загрузите файл CSV в книгу
            workbook = new Workbook(tempCsvFilePath, loadOptions);

            // Сохраните Workbook в файл Excel
            workbook.Save("TxtLoadStyleStrategyExample.xlsx");

            // Очистите временный файл CSV
            System.IO.File.Delete(tempCsvFilePath);

            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



---
title: "Перечисление CopyFormatType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.CopyFormatType. Представляет тип формата копирования при вставке строк"
type: docs
url: /ru/net/aspose.cells/copyformattype/
---
## CopyFormatType enumeration

Представляет тип копирования формата при вставке строк.

```csharp
public enum CopyFormatType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| SameAsAbove | `0` | Форматы такие же, как в строке выше. |
| SameAsBelow | `1` | Форматы такие же, как в строке ниже. |
| Clear | `2` | Очищает форматирование. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CopyFormatTypeDemo
    {
        public static void CopyFormatTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторые данные в листе
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");

            // Создайте InsertOptions и задайте CopyFormatType
            InsertOptions insertOptions = new InsertOptions();
            insertOptions.CopyFormatType = CopyFormatType.SameAsAbove;

            // Вставьте строку на вторую позицию с указанным типом формата
            worksheet.Cells.InsertRows(1, 1, insertOptions);

            // Сохраните книгу
            workbook.Save("CopyFormatTypeExample.xlsx");
            workbook.Save("CopyFormatTypeExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



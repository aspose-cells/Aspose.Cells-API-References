---
title: "Перечисление PrintErrorsType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.PrintErrorsType. Представляет константы ошибок печати"
type: docs
url: /ru/net/aspose.cells/printerrorstype/
---
## PrintErrorsType enumeration

Представляет константы ошибок печати.

```csharp
public enum PrintErrorsType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| PrintErrorsBlank | `0` | Представляет отсутствие печати ошибок. |
| PrintErrorsDash | `1` | Представляет печать ошибок как "--". |
| PrintErrorsDisplayed | `2` | Представляет печать ошибок в отображаемом виде. |
| PrintErrorsNA | `3` | Представляет печать ошибок как "#N/A". |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintErrorsTypeDemo
    {
        public static void PrintErrorsTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к PageSetup листа
            PageSetup pageSetup = worksheet.PageSetup;

            // Установить различные типы ошибок печати
            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            workbook.Save("PrintErrorsBlank.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            workbook.Save("PrintErrorsDash.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDisplayed;
            workbook.Save("PrintErrorsDisplayed.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsNA;
            workbook.Save("PrintErrorsNA.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



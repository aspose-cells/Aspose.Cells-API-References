---
title: "Класс ErrorCheckOption"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ErrorCheckOption. Настройка проверки ошибок, применяемая к определённым диапазонам"
type: docs
url: /ru/net/aspose.cells/errorcheckoption/
---
## ErrorCheckOption class

Настройка проверки ошибок, применяемая к определённым диапазонам.

```csharp
public class ErrorCheckOption
```

## Методы

| Имя | Описание |
| --- | --- |
| [AddRange](../../aspose.cells/errorcheckoption/addrange/)(CellArea) | Добавляет один затронутый диапазон этим параметром. |
| [GetCountOfRange](../../aspose.cells/errorcheckoption/getcountofrange/)() | Получает количество диапазонов, затронутых этим параметром. |
| [GetRange](../../aspose.cells/errorcheckoption/getrange/)(int) | Получает затронутый диапазон этого параметра по заданному индексу. |
| [IsErrorCheck](../../aspose.cells/errorcheckoption/iserrorcheck/)(ErrorCheckType) | Проверяет, будет ли проверяться указанный тип ошибки. |
| [RemoveRange](../../aspose.cells/errorcheckoption/removerange/)(int) | Удаляет один диапазон по заданному индексу. |
| [SetErrorCheck](../../aspose.cells/errorcheckoption/seterrorcheck/)(ErrorCheckType, bool) | Устанавливает, будет ли проверяться указанный тип ошибки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckOptionDemo
    {
        public static void ErrorCheckOptionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получите ErrorCheckOptionCollection из листа
            ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;

            // Добавьте новый ErrorCheckOption в коллекцию
            int optionIdx = opts.Add();
            ErrorCheckOption opt = opts[optionIdx];

            // Установите параметры проверки ошибок
            opt.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            opt.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            opt.SetErrorCheck(ErrorCheckType.TextDate, false);
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.SetErrorCheck(ErrorCheckType.Validation, false);

            // Определите область ячеек и добавьте её в ErrorCheckOption
            CellArea ca = CellArea.CreateCellArea("A1", "B10");
            opt.AddRange(ca);

            // Сохраните книгу
            workbook.Save("ErrorCheckOptionExample.xlsx");
            workbook.Save("ErrorCheckOptionExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



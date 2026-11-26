---
title: "Перечисление ErrorCheckType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ErrorCheckType. Представляет все типы проверки ошибок"
type: docs
url: /ru/net/aspose.cells/errorchecktype/
---
## ErrorCheckType enumeration

Представляет все типы проверки ошибок.

```csharp
public enum ErrorCheckType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| EvaluationError | `1` | Игнорировать ошибки, когда ячейки содержат формулы, приводящие к ошибке. |
| Calc | `1` |  |
| EmptyCellRef | `2` | Игнорировать ошибки, когда формулы ссылаются на пустые ячейки. |
| NumberStoredAsText | `4` | Игнорировать ошибки, когда числа отформатированы как текст или предшествует им апостроф |
| TextNumber | `4` | Игнорировать ошибки, когда числа отформатированы как текст или предшествует им апостроф |
| InconsistRange | `8` | Игнорировать ошибки, когда формулы пропускают определённые ячейки в области. |
| InconsistFormula | `16` | Игнорировать ошибки, когда формула в области вашего листа отличается от других формул в той же области. |
| TwoDigitTextYear | `32` | Игнорировать ошибки, когда формулы содержат ячейки с текстовым форматом, где годы представлены двумя цифрами. |
| TextDate | `32` | Игнорировать ошибки, когда формулы содержат ячейки с текстовым форматом, где годы представлены двумя цифрами. |
| UnlockedFormula | `64` | Игнорировать ошибки, когда разблокированные ячейки содержат формулы. |
| UnproctedFormula | `64` | Игнорировать ошибки, когда разблокированные ячейки содержат формулы. |
| TableDataValidation | `128` | Игнорировать ошибки, когда значение ячейки в таблице не соответствует указанным правилам проверки данных. |
| Validation | `128` | Игнорировать ошибки, когда значение ячейки в таблице не соответствует указанным правилам проверки данных. |
| CalculatedColumn | `129` | Игнорировать ошибки, когда ячейки содержат значение, отличное от формулы вычисляемого столбца. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckTypeDemo
    {
        public static void ErrorCheckTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к ErrorCheckOptionCollection
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;

            // Добавить новый ErrorCheckOption
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];

            // Установить различные типы проверки ошибок в false
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.Validation, false);

            // Определить область ячеек для параметра проверки ошибок.
            CellArea cellArea = CellArea.CreateCellArea("A1", "B10");
            errorCheckOption.AddRange(cellArea);

            // Сохраните книгу
            workbook.Save("ErrorCheckTypeExample.xlsx");
            workbook.Save("ErrorCheckTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



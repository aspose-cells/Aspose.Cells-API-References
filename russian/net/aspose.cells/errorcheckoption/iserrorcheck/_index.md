---
title: "ErrorCheckOption.IsErrorCheck"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ErrorCheckOption. Проверяет, будет ли проверяться указанный тип ошибки"
type: docs
url: /ru/net/aspose.cells/errorcheckoption/iserrorcheck/
---
## ErrorCheckOption.IsErrorCheck method

Проверяет, будет ли проверяться указанный тип ошибки.

```csharp
public bool IsErrorCheck(ErrorCheckType errorCheckType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | можно проверять тип ошибки |

### Возвращаемое значение

возвращает true, если указанный тип ошибки будет проверяться (зеленый треугольник будет отображён в ячейке, если проверка не удалась).

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodIsErrorCheckWithErrorCheckTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
            int index = options.Add();
            ErrorCheckOption option = options[index];

            // Настройте параметры проверки ошибок
            option.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            option.SetErrorCheck(ErrorCheckType.EvaluationError, true);
            option.SetErrorCheck(ErrorCheckType.InconsistRange, false);

            // Добавить диапазон для применения этих настроек
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 10;
            area.StartColumn = 0;
            area.EndColumn = 5;
            option.AddRange(area);

            // Проверить и отобразить настройки
            Console.WriteLine("NumberStoredAsText check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.NumberStoredAsText));
            Console.WriteLine("EvaluationError check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.EvaluationError));
            Console.WriteLine("InconsistRange check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.InconsistRange));
        }
    }
}
```

### См. также

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



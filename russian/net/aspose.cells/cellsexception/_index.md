---
title: "Класс CellsException"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CellsException. Исключение, которое выбрасывается, когда происходит указанная ошибка Aspose.Cells"
type: docs
url: /ru/net/aspose.cells/cellsexception/
---
## CellsException class

Исключение, которое выбрасывается при возникновении указанной ошибки Aspose.Cells.

```csharp
public class CellsException : ApplicationException
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Code](../../aspose.cells/cellsexception/code/) { get; } | Представляет пользовательский код исключения. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;
    using System.Collections;

    public class CellsExceptionDemo
    {
        public static void CellsExceptionExample()
        {
            try
            {
                // Смоделируйте операцию, вызывающую исключение
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                // Преднамеренно вызываем исключение, получая доступ к недопустимой ячейке
                Cell cell = worksheet.Cells["InvalidCellAddress"];
            }
            catch (CellsException ex)
            {
                // Обработать CellsException
                Console.WriteLine("Aspose.Cells.CellsException caught!");
                Console.WriteLine($"Code: {ex.Code}");
                Console.WriteLine($"Message: {ex.Message}");
                Console.WriteLine($"TargetSite: {ex.TargetSite}");
                Console.WriteLine($"StackTrace: {ex.StackTrace}");
                Console.WriteLine($"HelpLink: {ex.HelpLink}");
                Console.WriteLine($"Source: {ex.Source}");
                Console.WriteLine($"HResult: {ex.HResult}");
                if (ex.InnerException != null)
                {
                    Console.WriteLine($"InnerException: {ex.InnerException.Message}");
                }
                foreach (DictionaryEntry entry in ex.Data)
                {
                    Console.WriteLine($"Data: {entry.Key} = {entry.Value}");
                }
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



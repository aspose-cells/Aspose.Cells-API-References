---
title: "CellsException.Code"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellsException. Представляет пользовательский код исключения"
type: docs
url: /ru/net/aspose.cells/cellsexception/code/
---
## CellsException.Code property

Представляет пользовательский код исключения.

```csharp
public ExceptionType Code { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsExceptionPropertyCodeDemo
    {
        public static void Run()
        {
            try
            {
                // Создать книгу и попытаться получить доступ к несуществующему листу
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets["NonExistentSheet"];
            }
            catch (CellsException e)
            {
                // Продемонстрировать использование свойства Code
                Console.WriteLine($"Error Code: {e.Code}");
                Console.WriteLine($"Error Message: {e.Message}");
            }
        }
    }
}
```

### См. также

* enum [ExceptionType](../../exceptiontype/)
* class [CellsException](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



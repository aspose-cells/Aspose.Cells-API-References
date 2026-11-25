---
title: "CellsException.Code"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellsException. Rappresenta il codice di eccezione personalizzato"
type: docs
url: /it/net/aspose.cells/cellsexception/code/
---
## CellsException.Code property

Rappresenta il codice di eccezione personalizzato.

```csharp
public ExceptionType Code { get; }
```

### Esempi

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
                // Crea una cartella di lavoro e prova ad accedere a un foglio non esistente
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets["NonExistentSheet"];
            }
            catch (CellsException e)
            {
                // Dimostrare l'uso della proprietà Code
                Console.WriteLine($"Error Code: {e.Code}");
                Console.WriteLine($"Error Message: {e.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [ExceptionType](../../exceptiontype/)
* class [CellsException](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



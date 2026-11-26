---
title: "CellsException.Code"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de CellsException. Representa el código de excepción personalizado"
type: docs
url: /es/net/aspose.cells/cellsexception/code/
---
## CellsException.Code property

Representa un código de excepción personalizado.

```csharp
public ExceptionType Code { get; }
```

### Ejemplos

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
                // Crear un libro de trabajo y intentar acceder a una hoja de cálculo que no existe
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets["NonExistentSheet"];
            }
            catch (CellsException e)
            {
                // Demostrar el uso de la propiedad Code
                Console.WriteLine($"Error Code: {e.Code}");
                Console.WriteLine($"Error Message: {e.Message}");
            }
        }
    }
}
```

### Ver también

* enum [ExceptionType](../../exceptiontype/)
* class [CellsException](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Clase CellsException"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.CellsException. La excepción que se lanza cuando ocurre un error especificado de Aspose.Cells"
type: docs
url: /es/net/aspose.cells/cellsexception/
---
## CellsException class

La excepción que se lanza cuando ocurre un error especificado de Aspose.Cells.

```csharp
public class CellsException : ApplicationException
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Code](../../aspose.cells/cellsexception/code/) { get; } | Representa un código de excepción personalizado. |

### Ejemplos

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
                // Simular una operación que cause una excepción
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                // Provocar intencionalmente una excepción al acceder a una celda no válida
                Cell cell = worksheet.Cells["InvalidCellAddress"];
            }
            catch (CellsException ex)
            {
                // Manejar la CellsException
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

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



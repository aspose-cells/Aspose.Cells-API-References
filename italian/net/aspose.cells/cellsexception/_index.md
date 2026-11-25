---
title: "Classe CellsException"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.CellsException. L'eccezione che viene lanciata quando si verifica un errore specificato da Aspose.Cells"
type: docs
url: /it/net/aspose.cells/cellsexception/
---
## CellsException class

L'eccezione che viene generata quando si verifica un errore specificato da **Aspose.Cells**.

```csharp
public class CellsException : ApplicationException
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Code](../../aspose.cells/cellsexception/code/) { get; } | Rappresenta il codice di eccezione personalizzato. |

### Esempi

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
                // Simula un'operazione che genera un'eccezione
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                // Causare intenzionalmente un'eccezione accedendo a una cella non valida
                Cell cell = worksheet.Cells["InvalidCellAddress"];
            }
            catch (CellsException ex)
            {
                // Gestire l'eccezione CellsException
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

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



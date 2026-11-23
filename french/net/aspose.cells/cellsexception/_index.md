---
title: "Classe CellsException"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CellsException. L'exception qui est levée lorsqu'une erreur spécifiée par Aspose.Cells se produit"
type: docs
url: /fr/net/aspose.cells/cellsexception/
---
## CellsException class

L'exception qui est levée lorsqu'une erreur spécifiée d'Aspose.Cells se produit.

```csharp
public class CellsException : ApplicationException
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Code](../../aspose.cells/cellsexception/code/) { get; } | Représente un code d'exception personnalisé. |

### Exemples

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
                // Simulez une opération qui provoque une exception
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                // Provoquez intentionnellement une exception en accédant à une cellule invalide
                Cell cell = worksheet.Cells["InvalidCellAddress"];
            }
            catch (CellsException ex)
            {
                // Gérer l'exception CellsException
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

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



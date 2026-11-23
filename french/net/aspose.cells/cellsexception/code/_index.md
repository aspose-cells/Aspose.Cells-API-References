---
title: "CellsException.Code"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellsException. Représente le code d'exception personnalisé"
type: docs
url: /fr/net/aspose.cells/cellsexception/code/
---
## CellsException.Code property

Représente un code d'exception personnalisé.

```csharp
public ExceptionType Code { get; }
```

### Exemples

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
                // Créer un classeur et essayer d'accéder à une feuille de calcul inexistante
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets["NonExistentSheet"];
            }
            catch (CellsException e)
            {
                // Démontrer l'utilisation de la propriété Code
                Console.WriteLine($"Error Code: {e.Code}");
                Console.WriteLine($"Error Message: {e.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [ExceptionType](../../exceptiontype/)
* class [CellsException](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



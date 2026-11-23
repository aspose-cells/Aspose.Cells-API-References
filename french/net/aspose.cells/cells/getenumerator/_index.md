---
title: "Cells.GetEnumerator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Récupère l'énumérateur des cellules"
type: docs
url: /fr/net/aspose.cells/cells/getenumerator/
---
## Cells.GetEnumerator method

Obtient l'énumérateur des cellules.

```csharp
public IEnumerator GetEnumerator()
```

### Valeur de retour

L'énumérateur de cellules

### Remarques

Lors du parcours des éléments à l'aide de l'énumérateur retourné, la collection de cellules ne doit pas être modifiée (par exemple des opérations qui entraîneraient la création d'une nouvelle Cell/Row ou la suppression d'une Cell/Row existante). Sinon, l'énumérateur pourrait ne pas être capable de parcourir toutes les cellules correctement (certains éléments pourraient être parcourus plusieurs fois ou être ignorés).

### Exemples

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            
            // Obtenez l'énumérateur et parcourez les cellules
            IEnumerator enumerator = worksheet.Cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                if (cell.Value != null)
                {
                    Console.WriteLine($"{cell.Name}: {cell.Value}");
                }
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Range.GetEnumerator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Obtient l'énumérateur pour les cellules de cette plage"
type: docs
url: /fr/net/aspose.cells/range/getenumerator/
---
## Range.GetEnumerator method

Obtient l'énumérateur des cellules de cette `Range`.

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
    public class RangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir des données d'exemple
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Banana");
            worksheet.Cells["C2"].PutValue("Cherry");
            worksheet.Cells["C3"].PutValue("Date");

            // Obtenir la plage et énumérer les cellules
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C3");
            IEnumerator enumerator = range.GetEnumerator();
            
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine($"{cell.Name}: {cell.Value}");
            }
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



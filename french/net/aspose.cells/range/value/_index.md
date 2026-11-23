---
title: "Range.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient et définit la valeur de la plage"
type: docs
url: /fr/net/aspose.cells/range/value/
---
## Range.Value property

Obtient et définit la valeur de la plage.

```csharp
public object Value { get; set; }
```

### Remarques

Si la plage contient plusieurs cellules, l'objet retourné/appliqué doit être un tableau à deux dimensions.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une plage à partir de A1 couvrant 3 × 3 cellules
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");

            // Définir un tableau 2D comme valeur de la plage
            int[,] values = new int[3, 3] { { 1, 2, 3 }, { 4, 5, 6 }, { 7, 8, 9 } };
            range.Value = values;

            // Enregistrez le classeur
            workbook.Save("RangePropertyValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



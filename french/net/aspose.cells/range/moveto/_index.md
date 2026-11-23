---
title: "Range.MoveTo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Déplace la plage actuelle vers la plage de destination"
type: docs
url: /fr/net/aspose.cells/range/moveto/
---
## Range.MoveTo method

Déplace la plage actuelle vers la plage de destination.

```csharp
public void MoveTo(int destRow, int destColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destRow | Int32 | La ligne de départ de la plage de destination. |
| destColumn | Int32 | La colonne de départ de la plage de destination. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMoveToWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créez une plage d'exemple (A1:B2)
            Aspose.Cells.Range originalRange = worksheet.Cells.CreateRange("A1", "B2");
            
            // Mettez quelques données dans la plage à titre de démonstration
            originalRange[0, 0].PutValue("A1");
            originalRange[0, 1].PutValue("B1");
            originalRange[1, 0].PutValue("A2");
            originalRange[1, 1].PutValue("B2");
            
            // Déplacez la plage d'une ligne vers le bas (vers A2:B3)
            originalRange.MoveTo(originalRange.FirstRow + 1, originalRange.FirstColumn);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



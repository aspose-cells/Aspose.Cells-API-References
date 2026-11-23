---
title: "Range.UnMerge"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Annule la fusion des cellules fusionnées de cette plage"
type: docs
url: /fr/net/aspose.cells/range/unmerge/
---
## Range.UnMerge method

Démarque les cellules fusionnées de cette plage.

```csharp
public void UnMerge()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fusionner les cellules B2 à D4
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "D4");
            range.Merge();
            
            // Vérifiez si la cellule B2 est fusionnée avant de la désfusionner
            Console.WriteLine("Before UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
            
            // Désfusionner la plage
            range.UnMerge();
            
            // Vérifiez si la cellule B2 est fusionnée après la désfusion
            Console.WriteLine("After UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



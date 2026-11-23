---
title: "RangeCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode RangeCollection. Ajoute un élément Range à la collection"
type: docs
url: /fr/net/aspose.cells/rangecollection/add/
---
## RangeCollection.Add method

Ajoute un élément [`Range`](../../range/) à la collection.

```csharp
[Obsolete("Use RangeCollection.AddRange(Range) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(Range range)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| plage | Plage | Objet Range |

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode AddRange(). Cette méthode sera supprimée 6 mois plus tard, à compter de décembre 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeCollectionMethodAddWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une plage et l’ajouter à la collection
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // Insérer des lignes pour démontrer l’expansion de la plage
            worksheet.Cells.InsertRows(2, 2);
            
            Console.WriteLine("Range row count after insertion: " + cellRange.RowCount);
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



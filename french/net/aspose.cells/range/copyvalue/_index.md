---
title: "Range.CopyValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Copie la valeur de la cellule d'une plage source"
type: docs
url: /fr/net/aspose.cells/range/copyvalue/
---
## Range.CopyValue method

Copie la valeur de cellule depuis une plage source.

```csharp
public void CopyValue(Range range)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| range | Range | Objet source [`Range`](../). |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyValueWithRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul et obtenir la première feuille
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "SourceSheet";
            
            // Ajouter une autre feuille de calcul pour la destination
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "DestinationSheet";
            
            // Créer des données d'exemple dans la plage source
            Cells cellsSrc = sheetSrc.Cells;
            cellsSrc["A1"].PutValue("Source Data");
            cellsSrc["A2"].PutValue(10);
            cellsSrc["B2"].PutValue(20);
            cellsSrc["A3"].PutValue(30);
            cellsSrc["B3"].PutValue(40);
            
            // Créer des plages pour la source et la destination
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A2:B3");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("D2:E3");
            
            // Copier les valeurs de la plage source vers la plage destination
            rangeDest.CopyValue(rangeSrc);
            
            // Enregistrez le classeur
            workbook.Save("RangeCopyValueDemo.xlsx");
            
            Console.WriteLine("Values copied successfully from source range to destination range.");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



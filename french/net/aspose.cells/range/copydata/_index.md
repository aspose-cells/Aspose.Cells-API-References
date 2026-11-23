---
title: "Range.CopyData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Copie les données de cellule, y compris les formules, depuis une plage source"
type: docs
url: /fr/net/aspose.cells/range/copydata/
---
## Range.CopyData method

Copie les données de cellule (y compris les formules) depuis une plage source.

```csharp
public void CopyData(Range range)
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
    public class RangeMethodCopyDataWithRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenez la première feuille de calcul et ajoutez quelques données
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            sheetSrc.Cells["A1"].PutValue("Source Data");
            sheetSrc.Cells["B1"].PutValue(100);
            sheetSrc.Cells["A2"].PutValue("More Data");
            sheetSrc.Cells["B2"].PutValue(200);

            // Ajoutez une feuille de calcul de destination
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";

            // Créez les plages source et destination
            Aspose.Cells.Range rangeSrc = sheetSrc.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("C3:D4");

            // Copiez les données de la plage source vers la plage destination
            rangeDest.CopyData(rangeSrc);

            // Enregistrez le classeur
            workbook.Save("RangeCopyDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



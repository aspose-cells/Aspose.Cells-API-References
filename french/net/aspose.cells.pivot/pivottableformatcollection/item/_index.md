---
title: "PivotTableFormatCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTableFormatCollection. Obtient le format par l'index"
type: docs
url: /fr/net/aspose.cells.pivot/pivottableformatcollection/item/
---
## PivotTableFormatCollection indexer

Obtient le format par l'index.

```csharp
public PivotTableFormat this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("example.xlsx");

            // Actualiser tous les tableaux croisés dynamiques
            workbook.Worksheets.RefreshAll();
            Cells cells = workbook.Worksheets[0].Cells;

            // Accéder au premier tableau croisé dynamique
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];

            // Démontrez la propriété Item en accédant au premier PivotFormat
            pt.PivotFormats[0].PivotArea.OnlyData = false;
            workbook.Worksheets.RefreshAll();

            // Modifier les paramètres de format en utilisant la propriété Item
            pt.PivotFormats[0].PivotArea.OnlyLabel = true;
            workbook.Worksheets.RefreshAll();

            // Enregistrer le classeur modifié
            workbook.Save("modified_example.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTableFormat](../../pivottableformat/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



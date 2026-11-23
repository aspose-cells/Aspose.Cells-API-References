---
title: "Cells.CopyColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Copie les données et les formats d'une colonne entière"
type: docs
url: /fr/net/aspose.cells/cells/copycolumn/
---
## Cells.CopyColumn method

Copie les données et les formats d'une colonne entière.

```csharp
public void CopyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | Cellules | L'objet Source Cells contient les données et les formats à copier. |
| sourceColumnIndex | Int32 | Indice de la colonne source. |
| destinationColumnIndex | Int32 | Indice de la colonne de destination. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // Créer le classeur source et remplir les données
            Workbook wbSrc = new Workbook();
            Cells cellsSrc = wbSrc.Worksheets[0].Cells;
            cellsSrc[0, 255].PutValue(1);
            cellsSrc[1, 255].PutValue(true);
            cellsSrc[2, 255].PutValue("abc");
            cellsSrc[3, 255].PutValue(false);
            cellsSrc[65535, 255].PutValue(2.56);

            // Créer le classeur de destination
            Workbook wbDest = new Workbook();
            Cells cellsDest = wbDest.Worksheets[0].Cells;

            // Copier la colonne de la source vers la destination
            cellsDest.CopyColumn(cellsSrc, 255, 0);

            // Enregistrer le résultat
            wbDest.Save("outputCopyColumn.xlsx");
            
            Console.WriteLine("Column copied successfully.");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



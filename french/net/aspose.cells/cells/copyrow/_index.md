---
title: "Cells.CopyRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Copie les données et les formats d'une ligne entière"
type: docs
url: /fr/net/aspose.cells/cells/copyrow/
---
## Cells.CopyRow method

Copie les données et les formats d'une ligne entière.

```csharp
public void CopyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | Cellules | L'objet Source Cells contient les données et les formats à copier. |
| sourceRowIndex | Int32 | Indice de ligne source. |
| destinationRowIndex | Int32 | Indice de ligne de destination. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet1 = workbook.Worksheets[0];
            Cells cells1 = worksheet1.Cells;
            
            // Ajoutez des données à la première ligne
            cells1["A1"].PutValue("Source Data");
            cells1["B1"].PutValue(100);
            cells1["C1"].PutValue(DateTime.Now);
            
            // Créez la deuxième feuille de calcul
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            Cells cells2 = worksheet2.Cells;
            
            // Copiez la ligne de Sheet1 à Sheet2
            cells2.CopyRow(cells1, 0, 0);
            
            // Copiez la ligne au sein de Sheet1 vers de nouvelles positions
            cells1.CopyRow(cells1, 0, 1);
            cells1.CopyRow(cells1, 0, 2);
            
            // Enregistrez le classeur
            workbook.Save("CopyRowExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



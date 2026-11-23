---
title: "Cells.HideColumns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Masque plusieurs colonnes"
type: docs
url: /fr/net/aspose.cells/cells/hidecolumns/
---
## Cells.HideColumns method

Masque plusieurs colonnes.

```csharp
public void HideColumns(int column, int totalColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | Index de colonne. |
| totalColumns | Int32 | Numéro de colonne. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Remplir des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Masquer les colonnes 3 à 5 (indice basé sur zéro)
            int startColumn = 2; // Column C
            int columnCount = 3;  // Hide 3 columns
            cells.HideColumns(startColumn, columnCount);

            // Enregistrez le classeur
            workbook.Save("HideColumnsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



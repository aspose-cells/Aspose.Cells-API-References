---
title: "Cells.UnhideColumns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Affiche plusieurs colonnes"
type: docs
url: /fr/net/aspose.cells/cells/unhidecolumns/
---
## Cells.UnhideColumns method

Dévoile plusieurs colonnes.

```csharp
public void UnhideColumns(int column, int totalColumns, double width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | Index de colonne. |
| totalColumns | Int32 | Numéro de colonne |
| largeur | Double | Largeur de colonne. |

### Remarques

S'applique uniquement à la largeur des colonnes masquées.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUnhideColumnsWithInt32Int32DoubleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Masquez les colonnes 1-3 (index zéro) initialement
            worksheet.Cells.HideColumns(1, 3);

            try
            {
                // Affiche les colonnes à partir de l'index 1 (deuxième colonne), sur une largeur de 3 colonnes, définissez la largeur à 15.5
                worksheet.Cells.UnhideColumns(1, 3, 15.5);

                // Vérifiez les colonnes affichées en contrôlant leur largeur
                Console.WriteLine($"Column 1 width after unhiding: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine("Columns 1-3 successfully unhidden with specified width");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnhideColumns: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("UnhideColumnsWithWidthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Cells.GetColumnOriginalWidthPoint"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient la hauteur originale des colonnes en unité de point si la colonne est masquée"
type: docs
url: /fr/net/aspose.cells/cells/getcolumnoriginalwidthpoint/
---
## Cells.GetColumnOriginalWidthPoint method

Obtient la hauteur originale de la colonne en unité de point si la colonne est masquée

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnOriginalWidthPoint(int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | L'index de ligne. |

### Valeur de retour

Largeur de la colonne en vue normale.

### Remarques

REMARQUE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode Cells.GetColumnWidth(int ,bool , CellsUnitType ). Cette méthode sera supprimée 12 mois après avril 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnOriginalWidthPointWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Préparer le paramètre d'index de colonne
            int columnIndex = 0;

            try
            {
                // Obtenir la largeur originale de la colonne en points
                double originalWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width of column {columnIndex}: {originalWidth} points");

                // Modifier la largeur de la colonne
                cells.SetColumnWidth(columnIndex, 15);
                Console.WriteLine("Set new column width to 15 points");

                // Obtenir à nouveau la largeur originale pour démontrer qu'elle reste inchangée
                double unchangedWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width remains: {unchangedWidth} points");

                // Obtenir la largeur actuelle pour montrer la modification
                double currentWidth = cells.GetColumnWidth(columnIndex);
                Console.WriteLine($"Current column width: {currentWidth} points");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnOriginalWidthPoint method: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("GetColumnOriginalWidthPointDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



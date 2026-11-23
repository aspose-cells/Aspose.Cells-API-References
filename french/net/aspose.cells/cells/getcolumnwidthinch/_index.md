---
title: "Cells.GetColumnWidthInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient la largeur de la colonne spécifiée en vue normale, en unités de pouces"
type: docs
url: /fr/net/aspose.cells/cells/getcolumnwidthinch/
---
## Cells.GetColumnWidthInch method

Obtient la largeur de la colonne spécifiée en vue normale, en unités de pouces.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnWidthInch(int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | Indice de colonne |

### Valeur de retour

Largeur de la colonne

Largeur de la colonne en vue normale.

### Remarques

REMARQUE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode Cells.GetColumnWidth(int ,bool , CellsUnitType ). Cette méthode sera supprimée 12 mois après avril 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthInchWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir la largeur de la colonne en pouces pour la démonstration
            int columnIndex = 2;
            cells.SetColumnWidthInch(columnIndex, 2.5);

            try
            {
                // Appeler GetColumnWidthInch avec le paramètre Int32
                double columnWidth = cells.GetColumnWidthInch(columnIndex);

                // Afficher le résultat
                Console.WriteLine($"Width of column {columnIndex} in inches: {columnWidth}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthInch method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("CellsMethodGetColumnWidthInchDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



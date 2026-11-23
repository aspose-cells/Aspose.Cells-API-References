---
title: "Cells.GetCellStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtenir le style de la cellule donnée"
type: docs
url: /fr/net/aspose.cells/cells/getcellstyle/
---
## Cells.GetCellStyle method

Obtient le style de la cellule donnée.

```csharp
public Style GetCellStyle(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | index de ligne |
| column | Int32 | column |

### Valeur de retour

le style de la cellule donnée.

### Remarques

Le style retourné est uniquement celui défini pour la cellule ou hérité de la ligne/colonne de la cellule, il n'inclut pas les propriétés appliquées par d'autres paramètres tels que les mises en forme conditionnelles.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsMethodGetCellStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à la cellule B5 (ligne 4, colonne 1) et définissez le style initial
            Cell cell = worksheet.Cells["B5"];
            cell.PutValue("Styled Cell");
            
            // Créer et appliquer le style initial de la cellule
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.IsBold = true;  // Changed from Bold to IsBold
            initialStyle.BackgroundColor = Color.LightYellow;
            cell.SetStyle(initialStyle);

            try
            {
                // Appelez GetCellStyle avec des paramètres Int32 (ligne 4, colonne 1)
                Style cellStyle = worksheet.Cells.GetCellStyle(4, 1);

                // Afficher les propriétés du style récupéré
                Console.WriteLine($"Retrieved style - Bold: {cellStyle.Font.IsBold}, Background: {cellStyle.BackgroundColor}");  // Changed from Bold to IsBold

                // Modifier le style récupéré
                cellStyle.Font.IsItalic = true;  // Changed from Italic to IsItalic
                cellStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

                // Appliquer le style modifié à la cellule
                cell.SetStyle(cellStyle);

                Console.WriteLine("GetCellStyle executed successfully. Modified border and font style.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellStyle: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("CellsGetCellStyleWithInt32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "WorkbookSettings.UpdateAdjacentCellsBorder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Indique si la bordure des cellules adjacentes doit être mise à jour"
type: docs
url: /fr/net/aspose.cells/workbooksettings/updateadjacentcellsborder/
---
## WorkbookSettings.UpdateAdjacentCellsBorder property

Indique si la bordure des cellules adjacentes doit être mise à jour.

```csharp
public bool UpdateAdjacentCellsBorder { get; set; }
```

### Remarques

La valeur par défaut est false. Par exemple : la bordure inférieure de la cellule A1 est mise à jour, la bordure supérieure de la cellule A2 doit également être modifiée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateAdjacentCellsBorderDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Activer la mise à jour des bordures des cellules adjacentes
            workbook.Settings.UpdateAdjacentCellsBorder = true;

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir la valeur et appliquer la bordure à la cellule A1
            worksheet.Cells["A1"].PutValue("Sample");
            Style styleA1 = workbook.CreateStyle();
            styleA1.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            styleA1.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            worksheet.Cells["A1"].SetStyle(styleA1);

            // Définir la valeur à la cellule adjacente B1 (à droite de A1)
            worksheet.Cells["B1"].PutValue("Adjacent");

            // Enregistrez le classeur
            workbook.Save("output.xlsx");

            Console.WriteLine("Workbook saved with adjacent cell border update enabled.");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



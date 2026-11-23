---
title: "Workbook.RemoveUnusedStyles"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Supprime tous les styles inutilisés"
type: docs
url: /fr/net/aspose.cells/workbook/removeunusedstyles/
---
## Workbook.RemoveUnusedStyles method

Supprime tous les styles inutilisés.

```csharp
public void RemoveUnusedStyles()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveUnusedStylesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = wb.Worksheets[0];
            
            // Ajouter des données d'exemple avec des styles
            for (int i = 0; i < 10; i++)
            {
                Cell cell = sheet.Cells[i, 0];
                cell.PutValue("Item " + (i + 1));
                
                // Appliquer différents styles aux cellules
                Style style = wb.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 10 + i;
                style.Font.IsBold = i % 2 == 0;
                cell.SetStyle(style);
            }
            
            // Supprimer certaines cellules pour laisser des styles inutilisés
            sheet.Cells.DeleteRows(5, 5);
            
            // Enregistrer avant de supprimer les styles inutilisés
            wb.Save("BeforeRemoveUnusedStyles.xlsx");
            
            // Supprimer les styles inutilisés
            wb.RemoveUnusedStyles();
            
            // Enregistrer après avoir supprimé les styles inutilisés
            wb.Save("AfterRemoveUnusedStyles.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



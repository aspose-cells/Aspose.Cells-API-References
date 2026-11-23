---
title: "WorkbookSettings.SheetTabBarWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Largeur de la barre d'onglets de feuille de calcul en millièmes de la largeur de la fenêtre"
type: docs
url: /fr/net/aspose.cells/workbooksettings/sheettabbarwidth/
---
## WorkbookSettings.SheetTabBarWidth property

Largeur de la barre d'onglets de la feuille de calcul (en 1/1000 de la largeur de la fenêtre).

```csharp
public int SheetTabBarWidth { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySheetTabBarWidthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir la propriété SheetTabBarWidth
            workbook.Settings.SheetTabBarWidth = 1000;
            
            // Obtenir et afficher la valeur de SheetTabBarWidth
            Console.WriteLine("SheetTabBarWidth: " + workbook.Settings.SheetTabBarWidth);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "WorkbookSettings.IsVScrollBarVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient ou définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement verticale"
type: docs
url: /fr/net/aspose.cells/workbooksettings/isvscrollbarvisible/
---
## WorkbookSettings.IsVScrollBarVisible property

Obtient ou définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement verticale.

```csharp
public bool IsVScrollBarVisible { get; set; }
```

### Remarques

La valeur par défaut est true.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsVScrollBarVisibleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;
            
            // Masquer la barre de défilement verticale
            settings.IsVScrollBarVisible = false;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Vertical scroll bar visibility set to false. Workbook saved.");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



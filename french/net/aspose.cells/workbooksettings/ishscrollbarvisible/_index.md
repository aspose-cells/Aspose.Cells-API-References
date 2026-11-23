---
title: "WorkbookSettings.IsHScrollBarVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient ou définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement horizontale"
type: docs
url: /fr/net/aspose.cells/workbooksettings/ishscrollbarvisible/
---
## WorkbookSettings.IsHScrollBarVisible property

Obtient ou définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement horizontale.

```csharp
public bool IsHScrollBarVisible { get; set; }
```

### Remarques

La valeur par défaut est true.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHScrollBarVisibleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;
            
            // Masquer la barre de défilement horizontale
            settings.IsHScrollBarVisible = false;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with horizontal scroll bar hidden.");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



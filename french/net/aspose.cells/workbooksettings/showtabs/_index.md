---
title: "WorkbookSettings.ShowTabs"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient ou définit une valeur indiquant si les onglets du classeur sont affichés"
type: docs
url: /fr/net/aspose.cells/workbooksettings/showtabs/
---
## WorkbookSettings.ShowTabs property

Obtient ou définit une valeur indiquant si les onglets du classeur sont affichés.

```csharp
public bool ShowTabs { get; set; }
```

### Remarques

La valeur par défaut est true.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyShowTabsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Masquer les onglets de la feuille de calcul
            workbook.Settings.ShowTabs = false;
            
            // Enregistrez le classeur
            workbook.Save("HideTabsDemo.xlsx", SaveFormat.Xlsx);
            
            // Créer un autre classeur pour afficher les onglets
            Workbook workbook2 = new Workbook();
            
            // S'assurer que les onglets sont visibles (la valeur par défaut est true)
            workbook2.Settings.ShowTabs = true;
            
            // Enregistrez le classeur
            workbook2.Save("ShowTabsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



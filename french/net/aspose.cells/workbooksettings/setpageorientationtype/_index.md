---
title: "WorkbookSettings.SetPageOrientationType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorkbookSettings. Définit le type d'orientation d'impression pour l'ensemble du classeur"
type: docs
url: /fr/net/aspose.cells/workbooksettings/setpageorientationtype/
---
## WorkbookSettings.SetPageOrientationType method

Définit le type d'orientation d'impression pour l'ensemble du classeur.

```csharp
public void SetPageOrientationType(PageOrientationType pageOrientationType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageOrientationType | PageOrientationType | Le type d'orientation de page |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsMethodSetPageOrientationTypeWithPageOrientationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();
            
            // Définir l'orientation de page sur Portrait pour toutes les feuilles de calcul
            workbook.Settings.SetPageOrientationType(PageOrientationType.Portrait);
            
            // Vérifier que l'orientation est correctement définie
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine("Worksheet: " + sheet.Name + " - Orientation: " + sheet.PageSetup.Orientation);
            }
        }
    }
}
```

### Voir aussi

* enum [PageOrientationType](../../pageorientationtype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



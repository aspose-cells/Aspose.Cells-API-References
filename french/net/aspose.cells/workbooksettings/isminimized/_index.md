---
title: "WorkbookSettings.IsMinimized"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Représente si la feuille de calcul générée sera ouverte minimisée"
type: docs
url: /fr/net/aspose.cells/workbooksettings/isminimized/
---
## WorkbookSettings.IsMinimized property

Représente si la feuille de calcul générée sera ouverte minimisée.

```csharp
public bool IsMinimized { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsMinimizedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Définir la propriété IsMinimized sur true
            workbook.Settings.IsMinimized = true;

            // Enregistrez le classeur
            workbook.Save("IsMinimizedDemo.xlsx");

            // Chargez le classeur enregistré pour vérifier la propriété
            Workbook loadedWorkbook = new Workbook("IsMinimizedDemo.xlsx");

            // Afficher la valeur de la propriété IsMinimized
            Console.WriteLine("Workbook IsMinimized property: " + loadedWorkbook.Settings.IsMinimized);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



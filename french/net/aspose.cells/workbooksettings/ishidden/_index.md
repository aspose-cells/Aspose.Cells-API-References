---
title: "WorkbookSettings.IsHidden"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Indique si ce classeur est masqué"
type: docs
url: /fr/net/aspose.cells/workbooksettings/ishidden/
---
## WorkbookSettings.IsHidden property

Indique si ce workbook est masqué.

```csharp
public bool IsHidden { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;

            // Définissez la propriété IsHidden sur true
            settings.IsHidden = true;
            Console.WriteLine("Workbook is hidden: " + settings.IsHidden);

            // Enregistrez le classeur
            workbook.Save("WorkbookSettings_IsHidden_True.xlsx");

            // Créez un autre classeur
            Workbook workbook2 = new Workbook();

            // Accéder aux paramètres du classeur
            WorkbookSettings settings2 = workbook2.Settings;

            // Définissez la propriété IsHidden sur false (par défaut)
            settings2.IsHidden = false;
            Console.WriteLine("Workbook is hidden: " + settings2.IsHidden);

            // Enregistrez le classeur
            workbook2.Save("WorkbookSettings_IsHidden_False.xlsx");

            // Chargez et vérifiez les classeurs enregistrés
            Workbook loadedWorkbook1 = new Workbook("WorkbookSettings_IsHidden_True.xlsx");
            Console.WriteLine("Loaded workbook1 is hidden: " + loadedWorkbook1.Settings.IsHidden);

            Workbook loadedWorkbook2 = new Workbook("WorkbookSettings_IsHidden_False.xlsx");
            Console.WriteLine("Loaded workbook2 is hidden: " + loadedWorkbook2.Settings.IsHidden);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



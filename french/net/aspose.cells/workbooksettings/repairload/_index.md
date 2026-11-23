---
title: "WorkbookSettings.RepairLoad"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Indique si l'application a ouvert le classeur en mode sécurisé ou de réparation lors de la dernière ouverture"
type: docs
url: /fr/net/aspose.cells/workbooksettings/repairload/
---
## WorkbookSettings.RepairLoad property

Indique si l'application a ouvert le classeur en dernier en mode sécurisé ou de réparation.

```csharp
public bool RepairLoad { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRepairLoadDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Configurer les paramètres du classeur
            workbook.Settings.AutoRecover = false;
            workbook.Settings.DataExtractLoad = true;
            workbook.Settings.CrashSave = true;
            workbook.Settings.RepairLoad = true;

            // Enregistrez le classeur
            string outputPath = "WorkbookSettings_RepairLoad_Example.xlsx";
            workbook.Save(outputPath);

            // Charger le classeur enregistré pour vérifier les paramètres
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Afficher les paramètres dans la console
            Console.WriteLine("AutoRecover: " + loadedWorkbook.Settings.AutoRecover);
            Console.WriteLine("DataExtractLoad: " + loadedWorkbook.Settings.DataExtractLoad);
            Console.WriteLine("CrashSave: " + loadedWorkbook.Settings.CrashSave);
            Console.WriteLine("RepairLoad: " + loadedWorkbook.Settings.RepairLoad);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



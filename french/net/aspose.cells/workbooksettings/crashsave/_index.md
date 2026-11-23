---
title: "WorkbookSettings.CrashSave"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. indique si l'application a enregistré le fichier du classeur après un plantage"
type: docs
url: /fr/net/aspose.cells/workbooksettings/crashsave/
---
## WorkbookSettings.CrashSave property

Indique si l'application a enregistré le fichier du workbook après un plantage.

```csharp
public bool CrashSave { get; set; }
```

### Exemples

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCrashSaveDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("CrashSave Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;

            // Démontrer la propriété CrashSave
            settings.CrashSave = true;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // Enregistrer avec la sauvegarde après plantage activée
            workbook.Save("CrashSaveEnabled.xlsx");

            // Désactiver la sauvegarde après plantage
            settings.CrashSave = false;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // Enregistrer avec la sauvegarde après plantage désactivée
            workbook.Save("CrashSaveDisabled.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



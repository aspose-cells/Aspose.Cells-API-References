---
title: "WorkbookSettings.BuildVersion"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Spécifie la version publique incrémentielle de l'application"
type: docs
url: /fr/net/aspose.cells/workbooksettings/buildversion/
---
## WorkbookSettings.BuildVersion property

Spécifie la version publique incrémentielle de l'application.

```csharp
public string BuildVersion { get; set; }
```

### Exemples

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyBuildVersionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Définir les paramètres de base
            settings.Author = "Sample Author";
            settings.CultureInfo = new CultureInfo("en-US");
            
            // Démontrer la propriété BuildVersion
            settings.BuildVersion = "2.5.0";
            Console.WriteLine($"Build Version set to: {settings.BuildVersion}");
            
            // Enregistrez le classeur
            workbook.Save("BuildVersionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



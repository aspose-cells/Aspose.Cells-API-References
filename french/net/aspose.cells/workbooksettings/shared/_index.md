---
title: "WorkbookSettings.Shared"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient ou définit une valeur qui indique si le classeur est partagé"
type: docs
url: /fr/net/aspose.cells/workbooksettings/shared/
---
## WorkbookSettings.Shared property

Obtient ou définit une valeur indiquant si le classeur est partagé.

```csharp
public bool Shared { get; set; }
```

### Remarques

La valeur par défaut est false.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySharedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook book = new Workbook();
            
            // Définir la propriété Shared sur true
            book.Settings.Shared = true;
            
            // Enregistrez le classeur
            string outputPath = "output_shared.xlsx";
            book.Save(outputPath);
            
            // Charger le classeur enregistré pour vérifier la propriété Shared
            Workbook loadedBook = new Workbook(outputPath);
            Console.WriteLine("Shared property value: " + loadedBook.Settings.Shared);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



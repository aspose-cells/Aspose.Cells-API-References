---
title: "WorkbookSettings.UpdateLinksType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient et définit comment les liens externes sont mis à jour lorsque le classeur est ouvert"
type: docs
url: /fr/net/aspose.cells/workbooksettings/updatelinkstype/
---
## WorkbookSettings.UpdateLinksType property

Obtient et définit comment les liens externes sont mis à jour lorsque le classeur est ouvert.

```csharp
public UpdateLinksType UpdateLinksType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateLinksTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir UpdateLinksType sur Never
            workbook.Settings.UpdateLinksType = UpdateLinksType.Never;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Charger le classeur enregistré pour vérifier le paramètre
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Afficher la valeur de UpdateLinksType
            Console.WriteLine("UpdateLinksType: " + loadedWorkbook.Settings.UpdateLinksType);
        }
    }
}
```

### Voir aussi

* enum [UpdateLinksType](../../updatelinkstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



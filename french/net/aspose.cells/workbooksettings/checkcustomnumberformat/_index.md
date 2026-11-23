---
title: "WorkbookSettings.CheckCustomNumberFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Indique si la vérification du format numérique personnalisé est effectuée lors de la définition de Style.Custom"
type: docs
url: /fr/net/aspose.cells/workbooksettings/checkcustomnumberformat/
---
## WorkbookSettings.CheckCustomNumberFormat property

Indique si la vérification du format numérique personnalisé est effectuée lors du paramétrage de Style.Custom.

```csharp
public bool CheckCustomNumberFormat { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckCustomNumberFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            
            // Définissez d'abord un format numérique personnalisé valide
            style.Custom = "#,##0.00";
            
            // Activer la vérification stricte
            workbook.Settings.CheckCustomNumberFormat = true;
            
            try
            {
                // Tentative de définir un format numérique personnalisé invalide
                style.Custom = "fff @ ggg";
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error setting custom format: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



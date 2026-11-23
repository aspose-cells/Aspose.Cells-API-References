---
title: "WorkbookSettings.SmartTagOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient les options de la balise intelligente"
type: docs
url: /fr/net/aspose.cells/workbooksettings/smarttagoptions/
---
## WorkbookSettings.SmartTagOptions property

Obtient les options de la balise intelligente.

```csharp
public SmartTagOptions SmartTagOptions { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySmartTagOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();

                // Accéder aux paramètres du classeur
                WorkbookSettings settings = workbook.Settings;

                // Lisez la propriété SmartTagOptions
                var smartTagOptions = settings.SmartTagOptions;

                // Affichez les informations sur l'instance SmartTagOptions
                Console.WriteLine("SmartTagOptions instance type: " + smartTagOptions.GetType().FullName);

                // Optionnellement, vous pouvez inspecter l'état par défaut via `ToString()`
                Console.WriteLine("SmartTagOptions details: " + smartTagOptions.ToString());

                // Enregistrez le classeur (le fichier contiendra les paramètres par défaut)
                workbook.Save("SmartTagOptionsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SmartTagOptions](../../../aspose.cells.markup/smarttagoptions/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



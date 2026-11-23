---
title: "WarningInfo.Description"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WarningInfo. Obtient la description des informations d'avertissement"
type: docs
url: /fr/net/aspose.cells/warninginfo/description/
---
## WarningInfo.Description property

Obtenir la description des informations d'avertissement.

```csharp
public string Description { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyDescriptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez un nom défini en double pour déclencher un avertissement
            worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA";
            worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA"; // Different name to actually trigger warning

            // Obtenez le rappel d'avertissement
            WarningCallback callback = new WarningCallback();
            workbook.Settings.WarningCallback = callback; // Correct property path

            // Enregistrez pour déclencher un avertissement
            workbook.Save("output.xlsx");

            // Démontrez l'utilisation de la propriété Description
            if (callback.LastWarning != null)
            {
                Console.WriteLine("Warning Description: " + callback.LastWarning.Description);
                Console.WriteLine("Warning Type: " + callback.LastWarning.Type);
            }
        }
    }

    public class WarningCallback : IWarningCallback
    {
        public WarningInfo LastWarning { get; private set; }

        public void Warning(WarningInfo warningInfo)
        {
            LastWarning = warningInfo;
        }
    }
}
```

### Voir aussi

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



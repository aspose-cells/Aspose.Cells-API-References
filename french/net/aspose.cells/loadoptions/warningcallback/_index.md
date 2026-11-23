---
title: "LoadOptions.WarningCallback"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Obtient ou définit le rappel d'avertissement"
type: docs
url: /fr/net/aspose.cells/loadoptions/warningcallback/
---
## LoadOptions.WarningCallback property

Obtient ou définit le rappel d'avertissement.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.Description}");
        }
    }

    public class LoadOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Créer un rappel d'avertissement personnalisé
            IWarningCallback warningCallback = new CustomWarningCallback();

            // Initialiser les options de chargement avec le rappel d'avertissement
            LoadOptions options = new LoadOptions();
            options.WarningCallback = warningCallback;
            options.IgnoreUselessShapes = true;

            // Charger le classeur avec des options
            Workbook workbook = new Workbook("example.xlsx", options);

            // Démontrer l'utilisation du rappel d'avertissement en accédant à une cellule
            Console.WriteLine($"Cell value: {workbook.Worksheets[0].Cells["A1"].StringValue}");

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* interface [IWarningCallback](../../iwarningcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



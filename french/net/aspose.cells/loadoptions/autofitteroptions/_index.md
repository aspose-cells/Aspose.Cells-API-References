---
title: "LoadOptions.AutoFitterOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Obtient et définit les options d’ajustement automatique"
type: docs
url: /fr/net/aspose.cells/loadoptions/autofitteroptions/
---
## LoadOptions.AutoFitterOptions property

Obtient et définit les options d'ajustement automatique

```csharp
public AutoFitterOptions AutoFitterOptions { get; set; }
```

### Remarques

Uniquement pour les fichiers xlsx, SpreadsheetML pour le moment.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Créer AutoFitterOptions et définir les propriétés
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;
            options.OnlyAuto = false;

            // Créer LoadOptions et assigner AutoFitterOptions
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = options;

            // Charger le classeur avec les options spécifiées
            Workbook workbook = new Workbook("example.xlsx", loadOptions);

            // Démontrer l’ajustement automatique en obtenant la hauteur de ligne
            double rowHeight = workbook.Worksheets[0].Cells.GetRowHeight(0);
            Console.WriteLine("Row height after auto-fitting: " + rowHeight);
        }
    }
}
```

### Voir aussi

* class [AutoFitterOptions](../../autofitteroptions/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "AutoFitterOptions.FormatStrategy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AutoFitterOptions. Obtient et définit la stratégie de formatage"
type: docs
url: /fr/net/aspose.cells/autofitteroptions/formatstrategy/
---
## AutoFitterOptions.FormatStrategy property

Obtient et définit la stratégie de formatage.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Remarques

La valeur par défaut est CellStyle pour les performances.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir des données d'exemple et ajuster le texte
            worksheet.Cells["A1"].PutValue("Sample text for FormatStrategy demo");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Créer AutoFitterOptions avec FormatStrategy
            AutoFitterOptions options = new AutoFitterOptions
            {
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine
            };

            // Appliquer l'ajustement automatique avec les options spécifiées
            worksheet.AutoFitRows(options);

            // Enregistrer le résultat
            workbook.Save("FormatStrategyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



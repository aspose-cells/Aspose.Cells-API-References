---
title: "Classe InsertOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.InsertOptions classe. Représente les options d'insertion"
type: docs
url: /fr/net/aspose.cells/insertoptions/
---
## InsertOptions class

Représente les options d'insertion.

```csharp
public class InsertOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [InsertOptions](insertoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CopyFormatType](../../aspose.cells/insertoptions/copyformattype/) { get; set; } |  |
| [FormulaChangeMonitor](../../aspose.cells/insertoptions/formulachangemonitor/) { get; set; } | Obtient/définit le moniteur pour suivre les modifications causées par l'insertion. |
| [UpdateReference](../../aspose.cells/insertoptions/updatereference/) { get; set; } | Indique si les références dans d'autres feuilles de calcul seront mises à jour. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InsertOptionsDemo
    {
        public static void InsertOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une instance de InsertOptions
            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // Définissez la zone de cellules où les lignes seront insérées
            CellArea cellArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };

            // Insérez des lignes avec les options spécifiées
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            // Enregistrez le classeur
            workbook.Save("InsertOptionsExample.xlsx");
            workbook.Save("InsertOptionsExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



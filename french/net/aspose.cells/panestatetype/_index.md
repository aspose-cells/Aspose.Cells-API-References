---
title: "Énumération PaneStateType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.PaneStateType. Représente l'état du volet de la feuille"
type: docs
url: /fr/net/aspose.cells/panestatetype/
---
## PaneStateType enumeration

Représente l'état du volet de la feuille.

```csharp
public enum PaneStateType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Frozen | `0` | Les volets sont gelés, mais ne l'étaient pas avant d'être gelés. |
| FrozenSplit | `1` | Les volets sont gelés et étaient séparés avant d'être gelés. |
| Split | `2` | Les volets sont séparés, mais pas gelés. |
| Normal | `3` | Les volets ne sont ni gelés ni séparés. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PaneStateTypeDemo
    {
        public static void PaneStateTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir des données d'exemple dans la feuille de calcul
            worksheet.Cells["A1"].PutValue("Data 1");
            worksheet.Cells["A2"].PutValue("Data 2");
            worksheet.Cells["A3"].PutValue("Data 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Geler les volets à la cellule B2
            worksheet.FreezePanes(1, 0, 1, 1); // Freeze the first row and first column

            // Vérifier l'état du volet
            PaneStateType paneState = worksheet.PaneState;

            // Afficher l'état du volet
            Console.WriteLine("Current Pane State: " + paneState);

            // Enregistrez le classeur
            workbook.Save("PaneStateTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



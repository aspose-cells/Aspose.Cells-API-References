---
title: "Worksheet.PaneState"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Indique si le volet possède des divisions horizontales ou verticales et si ces divisions sont figées"
type: docs
url: /fr/net/aspose.cells/worksheet/panestate/
---
## Worksheet.PaneState property

Indique si le volet possède des séparations horizontales ou verticales, et si ces séparations sont figées.

```csharp
public PaneStateType PaneState { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPaneStateDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir des données d'exemple
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");

            // Figer les volets (première ligne)
            worksheet.FreezePanes(1, 0, 1, 0);

            // Obtenir et afficher l'état du volet
            PaneStateType paneState = worksheet.PaneState;
            Console.WriteLine("Pane State: " + paneState);

            // Enregistrer le classeur
            workbook.Save("PaneStateDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PaneStateType](../../panestatetype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



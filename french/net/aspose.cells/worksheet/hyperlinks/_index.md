---
title: "Worksheet.Hyperlinks"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient la collection HyperlinkCollection"
type: docs
url: /fr/net/aspose.cells/worksheet/hyperlinks/
---
## Worksheet.Hyperlinks property

Obtient la collection [`HyperlinkCollection`](../../hyperlinkcollection/).

```csharp
public HyperlinkCollection Hyperlinks { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHyperlinksDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez un hyperlien à la feuille de calcul
            worksheet.Hyperlinks.Add(0, 0, 1, 1, @"https://www.aspose.com");
            
            // Enregistrez le classeur
            workbook.Save("HyperlinksDemo.xlsx");
            
            // Chargez le classeur enregistré pour vérifier l'hyperlien
            Workbook loadedWorkbook = new Workbook("HyperlinksDemo.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Afficher l'adresse de l'hyperlien
            Console.WriteLine("Hyperlink Address: " + loadedWorksheet.Hyperlinks[0].Address);
        }
    }
}
```

### Voir aussi

* class [HyperlinkCollection](../../hyperlinkcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Worksheet.RemoveSplit"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Worksheet method. Supprime la fenêtre scindée"
type: docs
url: /fr/net/aspose.cells/worksheet/removesplit/
---
## Worksheet.RemoveSplit method

Supprime la fenêtre fractionnée.

```csharp
public void RemoveSplit()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveSplitDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Diviser la feuille de calcul
            worksheet.Split();
            Console.WriteLine("Worksheet split state: " + worksheet.PaneState);
            
            // Supprimer la division
            worksheet.RemoveSplit();
            Console.WriteLine("Worksheet split state after RemoveSplit: " + worksheet.PaneState);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



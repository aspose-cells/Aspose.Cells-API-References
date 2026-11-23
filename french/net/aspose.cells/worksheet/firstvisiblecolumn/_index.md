---
title: "Worksheet.FirstVisibleColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Représente l'index de la première colonne visible"
type: docs
url: /fr/net/aspose.cells/worksheet/firstvisiblecolumn/
---
## Worksheet.FirstVisibleColumn property

Représente l'index de la première colonne visible.

```csharp
public int FirstVisibleColumn { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Masquez la première colonne (index 0)
            worksheet.Cells.HideColumn(0);
            
            // Obtenir et afficher l'index de la première colonne visible
            Console.WriteLine("First visible column index: " + worksheet.FirstVisibleColumn);
            
            // Enregistrez le classeur
            workbook.Save("FirstVisibleColumnDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



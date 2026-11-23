---
title: "Worksheet.FirstVisibleRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Représente l'index de la première ligne visible"
type: docs
url: /fr/net/aspose.cells/worksheet/firstvisiblerow/
---
## Worksheet.FirstVisibleRow property

Représente l'index de la première ligne visible.

```csharp
public int FirstVisibleRow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir des données d'exemple
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // Définir la première ligne visible sur la ligne 20
            worksheet.FirstVisibleRow = 20;
            
            // Afficher la première ligne visible
            Console.WriteLine("First visible row: " + worksheet.FirstVisibleRow);
            
            // Enregistrez le classeur
            workbook.Save("FirstVisibleRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



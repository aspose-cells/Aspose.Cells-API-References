---
title: "Worksheet.ActiveCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient ou définit la cellule active dans la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/activecell/
---
## Worksheet.ActiveCell property

Obtient ou définit la cellule active dans la feuille de calcul.

```csharp
public string ActiveCell { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyActiveCellDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez la cellule active sur B2
            worksheet.ActiveCell = "B2";
            
            // Imprimer l'adresse de la cellule active
            Console.WriteLine("Active Cell: " + worksheet.ActiveCell);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Charger le classeur enregistré pour vérifier la cellule active
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Active Cell: " + loadedWorkbook.Worksheets[0].ActiveCell);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



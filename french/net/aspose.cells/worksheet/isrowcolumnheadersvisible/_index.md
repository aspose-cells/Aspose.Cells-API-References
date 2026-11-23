---
title: "Worksheet.IsRowColumnHeadersVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Worksheet property. Obtient ou définit une valeur indiquant si la feuille de calcul affichera les en-têtes de lignes et de colonnes. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/worksheet/isrowcolumnheadersvisible/
---
## Worksheet.IsRowColumnHeadersVisible property

Obtient ou définit une valeur indiquant si la feuille de calcul affichera les en-têtes de lignes et de colonnes. La valeur par défaut est true.

```csharp
public bool IsRowColumnHeadersVisible { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRowColumnHeadersVisibleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la visibilité des en-têtes de lignes et de colonnes sur false
            worksheet.IsRowColumnHeadersVisible = false;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Chargez le classeur enregistré pour vérifier la propriété
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Afficher la valeur de la propriété
            Console.WriteLine("Row and Column Headers Visible: " + loadedWorksheet.IsRowColumnHeadersVisible);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



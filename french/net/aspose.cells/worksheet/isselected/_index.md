---
title: "Worksheet.IsSelected"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Indique si cette feuille de calcul est sélectionnée lors de l'ouverture du classeur"
type: docs
url: /fr/net/aspose.cells/worksheet/isselected/
---
## Worksheet.IsSelected property

Indique si cette feuille de calcul est sélectionnée lorsque le classeur est ouvert.

```csharp
public bool IsSelected { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsSelectedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une deuxième feuille de calcul
            workbook.Worksheets.Add("Sheet2");
            
            // Obtenir la première feuille de calcul
            Worksheet worksheet1 = workbook.Worksheets[0];
            worksheet1.Name = "FirstSheet";
            
            // Obtenir la deuxième feuille de calcul
            Worksheet worksheet2 = workbook.Worksheets[1];
            worksheet2.Name = "SecondSheet";
            
            // Démontrer la propriété IsSelected
            Console.WriteLine("Before selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // Sélectionner la deuxième feuille de calcul
            worksheet2.IsSelected = true;
            workbook.Worksheets.ActiveSheetIndex = worksheet2.Index;
            
            Console.WriteLine("\nAfter selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // Enregistrez le classeur
            workbook.Save("WorksheetSelectionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



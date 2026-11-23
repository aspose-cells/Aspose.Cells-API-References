---
title: "Cell.IsTableFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Indique si cette cellule fait partie d'une formule de tableau"
type: docs
url: /fr/net/aspose.cells/cell/istableformula/
---
## Cell.IsTableFormula property

Indique si cette cellule fait partie d'une formule de tableau.

```csharp
public bool IsTableFormula { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellPropertyIsTableFormulaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer un tableau
            int index = worksheet.ListObjects.Add(0, 0, 5, 3, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Ajouter une formule de tableau à la cellule D2
            Cell cell = worksheet.Cells["D2"];
            cell.Formula = "=SUM(Table1[[#This Row],[Column1]:[Column3]])";
            
            // Vérifier si la cellule contient une formule de tableau
            Console.WriteLine("Is table formula: " + cell.IsTableFormula);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Cell.Formula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient ou définit une formule de la Cell"
type: docs
url: /fr/net/aspose.cells/cell/formula/
---
## Cell.Formula property

Obtient ou définit une formule du [`Cell`](../).

```csharp
public string Formula { get; set; }
```

### Remarques

Une chaîne de formule commence toujours par un signe égal (=). Et veuillez toujours utiliser la virgule (,) comme délimiteur de paramètres, par exemple "=SUM(A1, E1, H2)".

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez les valeurs dans les cellules qui seront utilisées dans la formule
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["E1"].PutValue(5);
            worksheet.Cells["A1"].PutValue(100);

            // Définissez la formule dans la cellule B6
            worksheet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + A1";

            // Calculer la formule
            workbook.CalculateFormula();

            // Afficher le résultat
            Console.WriteLine("Formula result in B6: " + worksheet.Cells["B6"].Value);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



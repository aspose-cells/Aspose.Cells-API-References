---
title: "Range.RefersTo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient les plages auxquelles il fait référence"
type: docs
url: /fr/net/aspose.cells/range/refersto/
---
## Range.RefersTo property

Obtient la référence de la plage.

```csharp
public string RefersTo { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRefersToDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données aux cellules
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Créer une plage nommée
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            
            // Définissez la propriété RefersTo pour la plage nommée
            name.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // Obtenez les plages référencées par le nom
            Aspose.Cells.Range[] ranges = name.GetRanges();
            
            // Affichez la propriété RefersTo de la première plage
            Console.WriteLine("Named range refers to: " + ranges[0].RefersTo);
            
            // Créez une formule qui utilise la plage nommée
            worksheet.Cells["B1"].Formula = "=SUM(MyRange)";
            
            // Calculer la formule
            Console.WriteLine("Sum of named range: " + worksheet.Cells["B1"].Value);
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



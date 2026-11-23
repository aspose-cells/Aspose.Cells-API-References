---
title: "Range.Worksheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient l'objet Worksheet qui contient cette plage"
type: docs
url: /fr/net/aspose.cells/range/worksheet/
---
## Range.Worksheet property

Obtient l'objet `Worksheet` qui contient cette plage.

```csharp
public Worksheet Worksheet { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyWorksheetDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une plage nommée
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            
            // Définissez une plage nommée
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1:$B$2";
            
            // Obtenez la plage par son nom (qualifiez pleinement Range pour éviter toute ambiguïté)
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("MyRange");
            
            // Démontrer l'utilisation de la propriété Worksheet
            Console.WriteLine("Range belongs to worksheet: " + range.Worksheet.Name);
            
            // Utiliser la propriété Worksheet pour modifier les cellules
            range.Worksheet.Cells["A1"].PutValue("Updated");
            
            // Enregistrez le classeur
            workbook.Save("RangePropertyWorksheetDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../worksheet/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



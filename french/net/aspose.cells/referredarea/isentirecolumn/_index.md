---
title: "ReferredArea.IsEntireColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ReferredArea. Indique si cette zone contient toutes les lignes de la colonne entière"
type: docs
url: /fr/net/aspose.cells/referredarea/isentirecolumn/
---
## ReferredArea.IsEntireColumn property

Indique si cette zone contient toutes les lignes (colonne entière).

```csharp
public bool IsEntireColumn { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertyIsEntireColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);

            // Créer une plage nommée faisant référence à la colonne entière B
            int index = workbook.Worksheets.Names.Add("PriceColumn");
            workbook.Worksheets.Names[index].RefersTo = "=Sheet1!$B:$B";

            // Obtenir la zone référencée de la plage nommée
            ReferredArea referredArea = workbook.Worksheets.Names["PriceColumn"].GetReferredAreas(false)[0];

            // Afficher la valeur de la propriété IsEntireColumn
            Console.WriteLine("IsEntireColumn value for PriceColumn: " + referredArea.IsEntireColumn);

            // Créer une autre plage nommée faisant référence à une plage spécifique (pas la colonne entière)
            int index2 = workbook.Worksheets.Names.Add("ProductRange");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1:$B$3";

            // Obtenir la zone référencée de la deuxième plage nommée
            ReferredArea referredArea2 = workbook.Worksheets.Names["ProductRange"].GetReferredAreas(false)[0];

            // Afficher la valeur de la propriété IsEntireColumn pour la deuxième plage
            Console.WriteLine("IsEntireColumn value for ProductRange: " + referredArea2.IsEntireColumn);

            // Démontrer l'effet de IsEntireColumn en vérifiant les dimensions de la plage
            Console.WriteLine("PriceColumn dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea.StartRow, referredArea.EndRow, referredArea.StartColumn, referredArea.EndColumn);

            Console.WriteLine("ProductRange dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea2.StartRow, referredArea2.EndRow, referredArea2.StartColumn, referredArea2.EndColumn);

            // Enregistrez le classeur
            workbook.Save("ReferredAreaPropertyIsEntireColumnDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



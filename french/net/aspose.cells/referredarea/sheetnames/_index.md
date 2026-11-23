---
title: "ReferredArea.SheetNames"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ReferredArea. Noms de toutes les feuilles de calcul auxquelles cette instance fait référence"
type: docs
url: /fr/net/aspose.cells/referredarea/sheetnames/
---
## ReferredArea.SheetNames property

Noms de toutes les feuilles de calcul auxquelles cette instance fait référence.

```csharp
public string[] SheetNames { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertySheetNamesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour créer une référence de formule
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Calculer les formules pour obtenir les références
            workbook.CalculateFormula();

            // Obtenir la zone référencée à partir de la formule en A3
            ReferredArea referredArea = worksheet.Cells["A3"].GetPrecedents()[0];

            // Afficher la propriété SheetNames
            Console.WriteLine("SheetNames referenced by the formula:");
            if (referredArea.SheetNames != null)
            {
                foreach (string sheetName in referredArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // Ajouter une autre feuille de calcul et créer une référence inter-feuilles
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["B1"].PutValue("=Sheet1!A3");

            // Recalculer les formules
            workbook.CalculateFormula();

            // Obtenez la zone référencée à partir de la formule inter-feuilles
            ReferredArea crossSheetArea = sheet2.Cells["B1"].GetPrecedents()[0];

            // Affichez les noms de feuilles pour la référence inter-feuilles
            Console.WriteLine("\nSheetNames referenced by cross-sheet formula:");
            if (crossSheetArea.SheetNames != null)
            {
                foreach (string sheetName in crossSheetArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // Enregistrez le classeur
            workbook.Save("ReferredAreaSheetNamesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



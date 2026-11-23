---
title: "CalculationOptions.LinkedDataSources"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationOptions. Spécifie les sources de données pour les liens externes utilisés dans les formules"
type: docs
url: /fr/net/aspose.cells/calculationoptions/linkeddatasources/
---
## CalculationOptions.LinkedDataSources property

Spécifie les sources de données pour les liens externes utilisés dans les formules.

```csharp
public Workbook[] LinkedDataSources { get; set; }
```

### Remarques

Comme [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/), vous pouvez spécifier ici les sources de données pour les liens externes utilisés dans les formules à calculer, en particulier ceux utilisés dans la fonction INDIRECT. Pour ces liens externes utilisés dans la fonction INDIRECT, ils ne sont pas considérés comme faisant partie des liens externes du classeur et ne peuvent pas être mis à jour par [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/). L'association de ces classeurs avec les liens externes est déterminée par [`FileName`](../../workbook/filename/) et [`DataSource`](../../externallink/datasource/). Veuillez donc vous assurer que [`FileName`](../../workbook/filename/) a été spécifié avec la valeur appropriée (généralement elle doit être identique à la [`DataSource`](../../externallink/datasource/) correspondante) pour chaque classeur afin qu'ils puissent être liés comme prévu.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyLinkedDataSourcesDemo
    {
        public static void Run()
        {
            // Créer un classeur externe avec des données
            Workbook wbExt = new Workbook();
            wbExt.Worksheets[0].Cells["A2"].PutValue(100);
            wbExt.Worksheets.Add("Sheet2").Cells["A2"].PutValue(200);
            
            // Ajouter des plages nommées dans le classeur externe
            int nameIndex1 = wbExt.Worksheets.Names.Add("Sheet1!ExtNamedRange1");
            wbExt.Worksheets.Names[nameIndex1].RefersTo = "=Sheet1!$A$2";
            int nameIndex2 = wbExt.Worksheets.Names.Add("Sheet2!ExtNamedRange2");
            wbExt.Worksheets.Names[nameIndex2].RefersTo = "=Sheet2!$A$2";
            int nameIndex3 = wbExt.Worksheets.Names.Add("GlobalNamedRange");
            wbExt.Worksheets.Names[nameIndex3].RefersTo = "=Sheet1!$A$2";

            // Créer le classeur principal
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Définir des formules qui font référence au classeur externe
            sheet.Cells["A1"].Formula = "=[External.xlsx]Sheet1!$A$2";
            sheet.Cells["A2"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!$A$2\")";
            sheet.Cells["A3"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!ExtNamedRange1\")";
            sheet.Cells["A4"].Formula = "=INDIRECT(\"[External.xlsx]!GlobalNamedRange\")";

            // Calculer les formules en utilisant LinkedDataSources
            CalculationOptions options = new CalculationOptions();
            options.LinkedDataSources = new Workbook[] { wbExt };
            
            Console.WriteLine("Before calculation:");
            PrintCellValues(sheet);

            wb.CalculateFormula(options);
            
            Console.WriteLine("\nAfter calculation:");
            PrintCellValues(sheet);
        }

        private static void PrintCellValues(Worksheet sheet)
        {
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {sheet.Cells[$"A{i+1}"].StringValue}");
            }
        }
    }
}
```

### Voir aussi

* class [Workbook](../../workbook/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



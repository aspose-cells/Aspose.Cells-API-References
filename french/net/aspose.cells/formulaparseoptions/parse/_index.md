---
title: "FormulaParseOptions.Parse"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormulaParseOptions. Indique si la formule donnée doit être analysée. La valeur par défaut est true. Si elle est false, la chaîne de formule donnée sera conservée telle quelle pour la cellule jusqu'à ce que l'utilisateur appelle d'autres méthodes pour l'analyser ou que les données de formule analysées soient requises par d'autres opérations telles que le calcul des formules."
type: docs
url: /fr/net/aspose.cells/formulaparseoptions/parse/
---
## FormulaParseOptions.Parse property

Indique s'il faut analyser la formule donnée. La valeur par défaut est true. Si elle est false, la chaîne de formule fournie sera conservée telle quelle pour la cellule jusqu'à ce que l'utilisateur appelle d'autres méthodes pour l'analyser ou que les données de formule analysée soient requises par d'autres opérations telles que le calcul des formules.

```csharp
public bool Parse { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyParseDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Définir les formules avec Parse=false (les formules ne seront pas analysées immédiatement)
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["B1"].SetFormula("=A1+A2", new FormulaParseOptions() { Parse = false });
            cells["B2"].SetFormula("=SUM(A1:A2)", new FormulaParseOptions() { Parse = false });

            // Calculer les formules (l'analyse se fera maintenant)
            wb.CalculateFormula();

            Console.WriteLine("B1 value: " + cells["B1"].Value);
            Console.WriteLine("B2 value: " + cells["B2"].Value);
        }
    }
}
```

### Voir aussi

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



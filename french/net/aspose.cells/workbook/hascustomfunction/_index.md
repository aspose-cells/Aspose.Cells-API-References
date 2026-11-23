---
title: "Workbook.HasCustomFunction"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété du classeur. Détecte si une fonction personnalisée est utilisée dans ce classeur, par exemple dans les formules des cellules ou les noms définis"
type: docs
url: /fr/net/aspose.cells/workbook/hascustomfunction/
---
## Workbook.HasCustomFunction property

Détecte s'il existe une fonction personnalisée utilisée dans ce classeur, comme dans la formule d'une cellule, dans les noms définis...

```csharp
public bool HasCustomFunction { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Ajouter une formule standard à un nom
            NameCollection names = wb.Worksheets.Names;
            int index = names.Add("StandardName");
            names[index].RefersTo = "=SUM(Sheet1!$A$1:$A$2)";
            Console.WriteLine($"Workbook has custom function (should be false): {wb.HasCustomFunction}");

            // Ajouter une fonction personnalisée à un nom
            index = names.Add("CustomName");
            names[index].RefersTo = "=MYFUNC()";
            Console.WriteLine($"Workbook has custom function (should be true): {wb.HasCustomFunction}");

            // Tester avec des formules de cellules
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Fonction standard dans la cellule
            cells["A1"].Formula = "=SUM(B1:B2)";
            Console.WriteLine($"Cell has custom function (should be false): {cells["A1"].HasCustomFunction}");

            // Fonction personnalisée dans la cellule
            cells["A2"].Formula = "=MYFUNC(B1)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A2"].HasCustomFunction}");

            // Référence à un nom avec fonction personnalisée
            cells["A3"].Formula = "=CustomName";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A3"].HasCustomFunction}");

            // Fonctions personnalisées combinées
            cells["A4"].Formula = "=MYFUNC(CustomName)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A4"].HasCustomFunction}");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



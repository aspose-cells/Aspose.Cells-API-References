---
title: "TxtLoadOptions.HasFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TxtLoadOptions. Indique si le texte est une formule s'il commence par"
type: docs
url: /fr/net/aspose.cells/txtloadoptions/hasformula/
---
## TxtLoadOptions.HasFormula property

Indique si le texte est une formule lorsqu'il commence par "=".

```csharp
public bool HasFormula { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // Créez des options de chargement de texte et activez l'analyse des formules
            TxtLoadOptions options = new TxtLoadOptions();
            options.HasFormula = true;
            options.SeparatorString = "|";

            // Chargez le classeur avec des formules dans le fichier texte
            Workbook workbook = new Workbook("example.csv", options);
            
            // Accédez à une cellule contenant une formule et affichez‑la
            Console.WriteLine("Cell K2 formula: " + workbook.Worksheets[0].Cells["K2"].Formula);
            
            // Enregistrez le classeur
            workbook.Save("example_output.xlsx");
        }
    }
}
```

### Voir aussi

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



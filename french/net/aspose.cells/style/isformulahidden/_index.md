---
title: "Style.IsFormulaHidden"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Représente si la formule sera masquée lorsque la feuille de calcul est protégée"
type: docs
url: /fr/net/aspose.cells/style/isformulahidden/
---
## Style.IsFormulaHidden property

Représente si la formule sera masquée lorsque la feuille de calcul est protégée.

```csharp
public bool IsFormulaHidden { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFormulaHiddenDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer un style avec IsFormulaHidden défini sur true
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;
            
            // Appliquer le style à une cellule
            cells["A1"].SetStyle(style);
            cells["A1"].Formula = "=1+1";

            // Créer un autre style avec IsFormulaHidden défini sur false
            Style style2 = workbook.CreateStyle();
            style2.IsFormulaHidden = false;
            
            // Appliquer le deuxième style à une autre cellule
            cells["B1"].SetStyle(style2);
            cells["B1"].Formula = "=2+2";

            // Protéger la feuille de calcul pour voir l'effet
            worksheet.Protect(ProtectionType.All, "password", null);

            // Enregistrez le classeur
            workbook.Save("IsFormulaHiddenDemo.xlsx");

            Console.WriteLine("Workbook saved with IsFormulaHidden examples.");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



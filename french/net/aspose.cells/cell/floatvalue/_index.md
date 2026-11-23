---
title: "Cell.FloatValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient la valeur flottante contenue dans la cellule"
type: docs
url: /fr/net/aspose.cells/cell/floatvalue/
---
## Cell.FloatValue property

Obtient la valeur flottante contenue dans la cellule.

```csharp
public float FloatValue { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFloatValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez la valeur numérique directement
            worksheet.Cells["A1"].PutValue(3.14f);
            Console.WriteLine("FloatValue of A1: " + worksheet.Cells["A1"].FloatValue);
            
            // Définissez une formule qui renvoie un flottant
            worksheet.Cells["A2"].Formula = "=3.5*2";
            workbook.CalculateFormula();
            Console.WriteLine("FloatValue of A2: " + worksheet.Cells["A2"].FloatValue);
            
            // Démontrez FloatValue avec une formule partagée
            worksheet.Cells["B1"].Formula = "=5-2";
            workbook.CalculateFormula();
            worksheet.Cells["B1"].SetSharedFormula("=5-2", 3, 1);
            workbook.CalculateFormula();
            Console.WriteLine("FloatValue of B3: " + worksheet.Cells["B3"].FloatValue);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



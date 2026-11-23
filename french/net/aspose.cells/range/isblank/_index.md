---
title: "Range.IsBlank"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Indique si la plage contient des valeurs"
type: docs
url: /fr/net/aspose.cells/range/isblank/
---
## Range.IsBlank method

Indique si la plage contient des valeurs.

```csharp
public bool IsBlank()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodIsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créez une plage et vérifiez si elle est vide (devrait être vrai)
            Aspose.Cells.Range range1 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank: " + range1.IsBlank());

            // Mettez une valeur dans une cellule et vérifiez à nouveau (devrait être faux)
            cells["B2"].PutValue("Test");
            Aspose.Cells.Range range2 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank after adding value: " + range2.IsBlank());
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



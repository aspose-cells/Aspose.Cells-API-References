---
title: "Range.Intersect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Retourne un objet Range qui représente l'intersection rectangulaire de deux plages"
type: docs
url: /fr/net/aspose.cells/range/intersect/
---
## Range.Intersect method

Retourne un objet [`Range`](../) qui représente l'intersection rectangulaire de deux plages.

```csharp
public Range Intersect(Range range)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| plage | Plage | La plage d'intersection. |

### Valeur de retour

Retourne un objet [`Range`](../)

### Remarques

Si les deux plages ne s'intersectent pas, retourne null.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodIntersectWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            Aspose.Cells.Range range1 = cells.CreateRange("A1:A5");
            Aspose.Cells.Range range2 = cells.CreateRange("A3:A10");
            
            Aspose.Cells.Range intersectRange = range1.Intersect(range2);
            
            Console.WriteLine("Intersected range: " + intersectRange.Address);
            workbook.Save("IntersectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



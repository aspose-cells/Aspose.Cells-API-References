---
title: "Range.GetOffset"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Obtient la plage Range par décalage"
type: docs
url: /fr/net/aspose.cells/range/getoffset/
---
## Range.GetOffset method

Obtient la plage [`Range`](../) par décalage.

```csharp
public Range GetOffset(int rowOffset, int columnOffset)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | Décalage de ligne dans cette plage, indexé à zéro. |
| columnOffset | Int32 | Décalage de colonne dans cette plage, indexé à zéro. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetOffsetWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Créez la plage initiale
            Aspose.Cells.Range originalRange = cells.CreateRange("A1");
            Console.WriteLine("Original Range Address: " + originalRange.Address);
            
            // Obtenez la plage décalée
            Aspose.Cells.Range offsetRange = originalRange.GetOffset(1, 1);
            Console.WriteLine("Offset Range Address: " + offsetRange.Address);
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



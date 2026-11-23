---
title: "Range.GetCellOrNull"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Obtient l'objet Cell ou null dans cette plage"
type: docs
url: /fr/net/aspose.cells/range/getcellornull/
---
## Range.GetCellOrNull method

Obtient l'objet [`Cell`](../../cell/) ou null dans cette plage.

```csharp
public Cell GetCellOrNull(int rowOffset, int columnOffset)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | Décalage de ligne dans cette plage, indexé à zéro. |
| columnOffset | Int32 | Décalage de colonne dans cette plage, indexé à zéro. |

### Valeur de retour

[`Cell`](../../cell/) object.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetCellOrNullWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une plage
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");
            
            // Remplissez des données dans la plage
            range[0, 0].PutValue("Cell A1");
            range[0, 1].PutValue("Cell B1");
            range[1, 0].PutValue("Cell A2");
            
            // Démontrez GetCellOrNull avec des paramètres Int32
            Cell cell1 = range.GetCellOrNull(0, 0);
            Console.WriteLine("Cell (0,0): " + (cell1 != null ? cell1.StringValue : "null"));
            
            Cell cell2 = range.GetCellOrNull(1, 1);
            Console.WriteLine("Cell (1,1): " + (cell2 != null ? cell2.StringValue : "null"));
            
            // Essayez d'obtenir une cellule en dehors de la plage (devrait retourner null)
            Cell cell3 = range.GetCellOrNull(2, 0);
            Console.WriteLine("Cell (2,0): " + (cell3 != null ? cell3.StringValue : "null"));
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



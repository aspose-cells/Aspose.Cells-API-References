---
title: "Cells.AddRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Ajoute une référence d'objet de plage aux cellules"
type: docs
url: /fr/net/aspose.cells/cells/addrange/
---
## Cells.AddRange method

Ajoute une référence d'objet de plage aux cellules

```csharp
public void AddRange(Range rangeObject)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rangeObject | Plage | L'objet de plage sera contenu dans les cellules |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodAddRangeWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définissez des données d'exemple dans la plage
            cells["A1"].PutValue("A1");
            cells["A2"].PutValue("A2");
            cells["B1"].PutValue("B1");
            cells["B2"].PutValue("B2");

            // Créez une plage et ajoutez-la en utilisant AddRange
            Aspose.Cells.Range range = cells.CreateRange("A1", "B2");
            cells.AddRange(range);

            // Modifiez la feuille de calcul pour démontrer l'expansion de la plage
            cells.InsertRow(1);
            cells.InsertColumn(1);

            Console.WriteLine($"Range now has {range.RowCount} rows and {range.ColumnCount} columns");
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



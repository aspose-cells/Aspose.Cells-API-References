---
title: "Range.FirstRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient l'index de la première ligne de la plage"
type: docs
url: /fr/net/aspose.cells/range/firstrow/
---
## Range.FirstRow property

Obtient l'index de la première ligne de la plage.

```csharp
public int FirstRow { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstRowDemo
    {
        public static void Run()
        {
            // Créez un classeur et accédez à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplissez quelques données
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Créez une plage
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Accédez et affichez la propriété FirstRow
            Console.WriteLine("First row index of range: " + range.FirstRow);

            // Accédez à la première cellule de la première ligne de la plage
            Cell firstCell = worksheet.Cells[range.FirstRow, range.FirstColumn];
            Console.WriteLine("First cell value: " + firstCell.StringValue);
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "ReferredArea.StartRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ReferredArea property. La ligne de début de la zone"
type: docs
url: /fr/net/aspose.cells/referredarea/startrow/
---
## ReferredArea.StartRow property

La ligne de départ de la zone.

```csharp
public int StartRow { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyStartRowDemo
    {
        public static void Run()
        {
            // Créez un classeur et une feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplissez quelques données d'exemple
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Créez une plage nommée qui fait référence à A2:A4
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$2:$A$4";

            // Obtenez la zone référencée avec le paramètre de recalcul
            ReferredArea area = name.GetReferredAreas(false)[0];

            // Démontrez la propriété StartRow
            Console.WriteLine("Start Row: " + area.StartRow); // Should output 1 (0-based)
            Console.WriteLine("End Row: " + area.EndRow);     // Should output 3 (0-based)
            Console.WriteLine("Row Count: " + (area.EndRow - area.StartRow + 1)); // Should output 3

            // Itérez à travers la zone référencée en utilisant StartRow et EndRow
            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                Cell cell = worksheet.Cells[row, 0]; // Column 0 is A
                Console.WriteLine("Value at row " + row + ": " + cell.Value);
            }
        }
    }
}
```

### Voir aussi

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



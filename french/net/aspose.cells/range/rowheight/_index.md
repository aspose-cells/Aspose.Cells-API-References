---
title: "Range.RowHeight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Définit ou obtient la hauteur des lignes dans cette plage"
type: docs
url: /fr/net/aspose.cells/range/rowheight/
---
## Range.RowHeight property

Définit ou obtient la hauteur des lignes dans cette plage

```csharp
public double RowHeight { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowHeightDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définissez des données dans la première ligne
            worksheet.Cells["A1"].PutValue("This is a test");
            worksheet.Cells["B1"].PutValue("to demonstrate");
            worksheet.Cells["C1"].PutValue("RowHeight property");

            // Obtenez la hauteur initiale de la ligne
            double initialHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Initial row height: " + initialHeight);

            // Ajustez automatiquement la ligne
            worksheet.AutoFitRow(0);

            // Obtenez la nouvelle hauteur de la ligne après l'ajustement automatique
            double newHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Row height after auto-fit: " + newHeight);

            // Définissez manuellement une nouvelle hauteur de ligne
            worksheet.Cells.CreateRange("1:1").RowHeight = 30;
            Console.WriteLine("Row height after manual set: " + worksheet.Cells.CreateRange("1:1").RowHeight);
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



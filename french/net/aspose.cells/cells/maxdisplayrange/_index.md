---
title: "Cells.MaxDisplayRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient la plage maximale qui inclut les cellules fusionnées de données et les formes"
type: docs
url: /fr/net/aspose.cells/cells/maxdisplayrange/
---
## Cells.MaxDisplayRange property

Obtient la plage maximale qui inclut les données, les cellules fusionnées et les formes.

```csharp
public Range MaxDisplayRange { get; }
```

### Remarques

Renvoie null si la feuille de calcul est vide depuis Aspose.Cells 21.5.2.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDisplayRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données aux cellules pour créer une plage d'affichage
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // Obtenez la plage d'affichage maximale
            Aspose.Cells.Range maxDisplayRange = worksheet.Cells.MaxDisplayRange;

            // Affichez les informations de la plage
            Console.WriteLine("Max Display Range:");
            Console.WriteLine($"Start Row: {maxDisplayRange.FirstRow}");
            Console.WriteLine($"Start Column: {maxDisplayRange.FirstColumn}");
            Console.WriteLine($"Total Rows: {maxDisplayRange.RowCount}");
            Console.WriteLine($"Total Columns: {maxDisplayRange.ColumnCount}");

            // Créez une nouvelle plage basée sur les dimensions de la plage d'affichage maximale
            Aspose.Cells.Range customRange = worksheet.Cells.CreateRange(
                maxDisplayRange.FirstRow,
                maxDisplayRange.FirstColumn,
                maxDisplayRange.RowCount,
                maxDisplayRange.ColumnCount);

            // Appliquez le formatage à la plage
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;
            customRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });

            // Enregistrez le classeur
            workbook.Save("MaxDisplayRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Cells.Columns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient la collection d'objets Column qui représente les colonnes individuelles de cette feuille de calcul"
type: docs
url: /fr/net/aspose.cells/cells/columns/
---
## Cells.Columns property

Obtient la collection d'objets [`Column`](../../column/) qui représente les colonnes individuelles de cette feuille de calcul.

```csharp
public ColumnCollection Columns { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyColumnsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir le style pour la colonne 5
            Style columnStyle = workbook.CreateStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 12;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { FontName = true, FontSize = true, FontBold = true });

            // Définir la largeur pour la colonne 5
            cells.Columns[5].Width = 20;

            // Définir des données dans la colonne 5 pour démontrer le style
            for (int row = 0; row < 10; row++)
            {
                cells[row, 5].PutValue($"Row {row + 1}");
            }

            // Enregistrez le classeur
            workbook.Save("ColumnsPropertyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ColumnCollection](../../columncollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



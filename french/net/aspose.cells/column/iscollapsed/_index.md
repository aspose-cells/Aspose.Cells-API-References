---
title: "Column.IsCollapsed"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Column. indique si la colonne est réduite"
type: docs
url: /fr/net/aspose.cells/column/iscollapsed/
---
## Column.IsCollapsed property

si la colonne est réduite

```csharp
public bool IsCollapsed { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIsCollapsedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer et appliquer un style simple à la colonne
            Style style = workbook.CreateStyle();
            style.BackgroundColor = Color.LightGray;
            
            Column column = worksheet.Cells.Columns[0];
            column.ApplyStyle(style, new StyleFlag { All = true });

            // Définir les propriétés de la colonne, y compris IsCollapsed
            column.Width = 15;
            column.IsCollapsed = true; // Demonstrating IsCollapsed property
            column.IsHidden = false;

            // Ajouter des données pour visualiser la colonne réduite
            worksheet.Cells["A1"].PutValue("Collapsed Column");
            worksheet.Cells["B1"].PutValue("Visible Column");

            workbook.Save("ColumnIsCollapsedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



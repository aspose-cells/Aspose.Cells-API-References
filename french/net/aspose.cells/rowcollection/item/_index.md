---
title: "RowCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RowCollection. Obtient un objet Row selon l'index de ligne fourni. L'objet Row de l'index donné sera instancié s'il n'existe pas auparavant."
type: docs
url: /fr/net/aspose.cells/rowcollection/item/
---
## RowCollection indexer

Obtient un objet [`Row`](../../row/) selon l'index de ligne fourni. L'objet Row de l'index donné sera instancié s'il n'existe pas auparavant.

```csharp
public Row this[int rowIndex] { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir la largeur standard pour les colonnes
            cells.StandardWidth = 20.0;

            // Accéder et styliser les lignes en utilisant la propriété Item
            for (int i = 0; i < 5; i++)
            {
                Row row = cells.Rows[i]; // Using Item property
                Style rowStyle = workbook.CreateStyle();
                rowStyle.Font.IsBold = true;
                rowStyle.Font.Color = System.Drawing.Color.Blue;
                row.ApplyStyle(rowStyle, new StyleFlag { Font = true });
                
                // Accéder et styliser la cellule dans la ligne
                Cell cell = cells[i, i]; // Using Cells indexer instead of row[i]
                cell.PutValue($"Row {i}, Col {i}");
                Style cellStyle = workbook.CreateStyle();
                cellStyle.BackgroundColor = System.Drawing.Color.LightYellow;
                cell.SetStyle(cellStyle);
            }

            // Enregistrez le classeur
            workbook.Save("RowCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



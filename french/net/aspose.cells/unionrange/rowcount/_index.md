---
title: "UnionRange.RowCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété UnionRange. Obtient le nombre de lignes dans la plage"
type: docs
url: /fr/net/aspose.cells/unionrange/rowcount/
---
## UnionRange.RowCount property

Obtient le nombre de lignes dans la plage.

```csharp
public int RowCount { get; }
```

### Remarques

N'affecte que lorsqu'il ne contient qu'une seule plage.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyRowCountDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplissez les données dans la feuille de calcul
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Data {row},{col}";
                }
            }

            // Créer une plage d'union de A1 à E5
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:E5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A6:E10");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Afficher la propriété RowCount
            Console.WriteLine("RowCount of union range: " + unionRange.RowCount);

            // Démontrer l'utilisation en parcourant les lignes
            for (int i = 0; i < unionRange.RowCount; i++)
            {
                Aspose.Cells.Range currentRow = worksheet.Cells.CreateRange(
                    unionRange.FirstRow + i,
                    unionRange.FirstColumn,
                    1,
                    unionRange.ColumnCount);

                Console.WriteLine($"Row {i + 1} first cell value: " + currentRow[0, 0].Value);
            }

            // Créer une nouvelle plage avec un nombre de lignes différent
            Aspose.Cells.Range newRange = worksheet.Cells.CreateRange("A1:E3");
            Console.WriteLine("RowCount of new range: " + newRange.RowCount);

            // Appliquer le formatage en fonction du nombre de lignes
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightYellow;
            style.Pattern = BackgroundType.Solid;

            for (int i = 0; i < unionRange.RowCount; i += 2)
            {
                Aspose.Cells.Range rowRange = worksheet.Cells.CreateRange(
                    unionRange.FirstRow + i,
                    unionRange.FirstColumn,
                    1,
                    unionRange.ColumnCount);
                rowRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });
            }

            // Enregistrez le classeur
            workbook.Save("UnionRangeRowCountDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



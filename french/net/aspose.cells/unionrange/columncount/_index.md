---
title: "UnionRange.ColumnCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété UnionRange. Obtient le nombre de lignes dans la plage"
type: docs
url: /fr/net/aspose.cells/unionrange/columncount/
---
## UnionRange.ColumnCount property

Obtient le nombre de lignes dans la plage.

```csharp
public int ColumnCount { get; }
```

### Remarques

N'affecte que lorsqu'il ne contient qu'une seule plage.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyColumnCountDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Laptop";
            worksheet.Cells["B2"].Value = 1200;
            worksheet.Cells["C2"].Value = 5;
            worksheet.Cells["A3"].Value = "Phone";
            worksheet.Cells["B3"].Value = 800;
            worksheet.Cells["C3"].Value = 10;

            try
            {
                // Créez des plages et combinez-les en une plage d'union
                Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C2");
                Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A3:C3");
                UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

                // Afficher la valeur de la propriété ColumnCount
                Console.WriteLine("ColumnCount of union range: " + unionRange.ColumnCount);

                // Démontrer l'utilisation en affichant les informations de colonne
                Console.WriteLine("First column index: " + unionRange.FirstColumn);
                Console.WriteLine("Last column index: " + (unionRange.FirstColumn + unionRange.ColumnCount - 1));

                // Créer une autre plage d'union avec un nombre de colonnes différent
                Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("A1:B2");
                Aspose.Cells.Range range4 = worksheet.Cells.CreateRange("D1:E2");
                UnionRange unionRange2 = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range3, range4 });

                // Comparer les nombres de colonnes
                Console.WriteLine("Second union range ColumnCount: " + unionRange2.ColumnCount);
                Console.WriteLine("First union range has " +
                    (unionRange.ColumnCount > unionRange2.ColumnCount ? "more" : "fewer") +
                    " columns than second union range");

                // Enregistrez le classeur
                workbook.Save("UnionRangeColumnCountDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



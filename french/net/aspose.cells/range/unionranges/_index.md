---
title: "Range.UnionRanges"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Retourne le résultat de l'union de deux plages"
type: docs
url: /fr/net/aspose.cells/range/unionranges/
---
## Range.UnionRanges method

Retourne le résultat de l'union de deux plages.

```csharp
public UnionRange UnionRanges(Range[] ranges)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| plages | Range[] | La plage |

### Valeur de retour

L'union de deux plages.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodUnionRangesWithRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez des données d'exemple dans les cellules
            worksheet.Cells["A1"].PutValue("Range 1");
            worksheet.Cells["B1"].PutValue("Data 1");
            worksheet.Cells["C1"].PutValue("Data 2");
            worksheet.Cells["A5"].PutValue("Range 2");
            worksheet.Cells["B5"].PutValue("Data 3");
            worksheet.Cells["C5"].PutValue("Data 4");

            // Créez des plages à unir
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C3");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A5:C7");

            try
            {
                // Appelez UnionRanges avec le paramètre Range[]
                Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range1, range2 };
                UnionRange unionRange = range1.UnionRanges(rangesToUnion);

                // Appliquez un style pour afficher la plage d'union
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });

                Console.WriteLine($"Union range created successfully. Address: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRanges method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("UnionRangesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [UnionRange](../../unionrange/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



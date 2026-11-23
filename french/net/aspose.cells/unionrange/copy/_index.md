---
title: "UnionRange.Copy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode UnionRange. Copie de la plage avec les options de collage spécial"
type: docs
url: /fr/net/aspose.cells/unionrange/copy/
---
## UnionRange.Copy method

Copie la plage avec les options de collage spécial.

```csharp
public void Copy(UnionRange range, PasteOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| plage | UnionRange | La plage source. |
| options | PasteOptions | Les options de collage spécial. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodCopyWithUnionRangePasteOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Source Data");
            worksheet.Cells["B1"].PutValue("Value1");
            worksheet.Cells["A2"].PutValue("More Data");
            worksheet.Cells["B2"].PutValue("Value2");

            try
            {
                // Créer l'UnionRange source
                UnionRange sourceRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(
                    new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

                // Créer l'UnionRange de destination
                UnionRange destinationRange = worksheet.Cells.CreateRange("D1:E2").UnionRanges(
                    new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("D1:E2") });

                // Créer PasteOptions avec des paramètres spécifiques
                PasteOptions options = new PasteOptions();
                options.PasteType = PasteType.All;
                options.SkipBlanks = true;
                options.Transpose = false;

                // Appeler la méthode Copy
                sourceRange.Copy(destinationRange, options);

                Console.WriteLine("Copy method executed successfully");
                Console.WriteLine($"Destination range: {destinationRange.RefersTo}");

                // Enregistrez le classeur
                workbook.Save("UnionRangeCopyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Copy: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PasteOptions](../../pasteoptions/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "UnionRange.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété UnionRange. Obtient ou définit le nom de la plage"
type: docs
url: /fr/net/aspose.cells/unionrange/name/
---
## UnionRange.Name property

Obtient ou définit le nom de la plage.

```csharp
public string Name { get; set; }
```

### Remarques

Les plages nommées sont prises en charge. Par exemple,

range.Name = "Sheet1!MyRange";

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].Value = "First Range";
            worksheet.Cells["B2"].Value = "Second Range";

            try
            {
                // Créez des plages et combinez-les en une plage d'union
                Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:A1");
                Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:B2");
                UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

                // Afficher la valeur actuelle de la propriété Name
                Console.WriteLine("Initial Name value: " + unionRange.Name);

                // Définir un nouveau nom pour la plage d'union
                unionRange.Name = "MyUnionRange";
                Console.WriteLine("Updated Name value: " + unionRange.Name);

                // Démontrer que le nom peut être changé à nouveau
                unionRange.Name = "CustomUnionRange";
                Console.WriteLine("Final Name value: " + unionRange.Name);

                // Enregistrez le classeur
                workbook.Save("UnionRangeNameDemo.xlsx");
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



---
title: "UnionRange.UnMerge"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode UnionRange. Démarque les cellules fusionnées de cette plage"
type: docs
url: /fr/net/aspose.cells/unionrange/unmerge/
---
## UnionRange.UnMerge method

Démarque les cellules fusionnées de cette plage.

```csharp
public void UnMerge()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une plage et fusionner les cellules
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
            
            // Fusionner les cellules et placer une valeur
            unionRange.Merge();
            unionRange.PutValue("Merged Cells", true, true);
            
            try
            {
                // Appeler la méthode UnMerge
                unionRange.UnMerge();
                
                Console.WriteLine("Cells unmerged successfully");
                
                // Placer des valeurs dans les cellules démarquées pour démontrer l'effet
                worksheet.Cells["A1"].PutValue("A1");
                worksheet.Cells["A2"].PutValue("A2");
                worksheet.Cells["B1"].PutValue("B1");
                worksheet.Cells["B2"].PutValue("B2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnMerge method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("MethodUnMergeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Range.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient ou définit le nom de la plage"
type: docs
url: /fr/net/aspose.cells/range/name/
---
## Range.Name property

Obtient ou définit le nom de la plage.

```csharp
public string Name { get; set; }
```

### Remarques

Les plages nommées sont prises en charge. Par exemple,

range.Name = "Sheet1!MyRange";

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créez une plage (colonnes A à B)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, true);
            
            // Définissez la propriété de nom pour la plage
            range.Name = "testRange";
            
            // Vérifiez que le nom a été défini
            Console.WriteLine("Range name: " + range.Name);
            
            // Enregistrez le classeur
            workbook.Save("RangeWithName.xlsx");
            
            // Ouvrez le fichier enregistré pour démontrer que le nom persiste
            Workbook loadedWorkbook = new Workbook("RangeWithName.xlsx");
            Aspose.Cells.Range loadedRange = loadedWorkbook.Worksheets[0].Cells.CreateRange(0, 2, true);
            Console.WriteLine("Loaded range name: " + loadedRange.Name);
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



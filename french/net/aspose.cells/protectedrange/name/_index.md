---
title: "ProtectedRange.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ProtectedRange property. Obtient le titre de la plage. Ceci est utilisé comme un descripteur et non comme une définition de plage nommée"
type: docs
url: /fr/net/aspose.cells/protectedrange/name/
---
## ProtectedRange.Name property

Obtient le titre de la plage. Il est utilisé comme un descripteur, pas comme une définition de plage nommée.

```csharp
public string Name { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une collection de plages protégées
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // Ajouter une plage protégée avec le nom "MyRange"
            int index = allowRanges.Add("MyRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];
            protectedRange.Password = "123";

            // Accéder et afficher la propriété Name
            Console.WriteLine("Protected range name: " + protectedRange.Name);
            Console.WriteLine("Cell area: {0},{1} to {2},{3}", 
                protectedRange.CellArea.StartRow,
                protectedRange.CellArea.StartColumn,
                protectedRange.CellArea.EndRow,
                protectedRange.CellArea.EndColumn);

            // Ajouter une autre plage nommée
            index = allowRanges.Add("SecondRange", 3, 3, 5, 5);
            ProtectedRange secondRange = allowRanges[index];
            Console.WriteLine("Second protected range name: " + secondRange.Name);

            // Enregistrez le classeur
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



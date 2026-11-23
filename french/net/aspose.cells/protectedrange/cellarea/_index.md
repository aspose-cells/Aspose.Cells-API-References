---
title: "ProtectedRange.CellArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ProtectedRange. Obtient l'objet CellArea qui représente la zone de cellules à protéger"
type: docs
url: /fr/net/aspose.cells/protectedrange/cellarea/
---
## ProtectedRange.CellArea property

Obtient l'objet `CellArea` qui représente la zone de cellules à protéger.

```csharp
public CellArea CellArea { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyCellAreaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des plages protégées
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;
            
            // Ajouter la première plage protégée
            int index1 = allowRanges.Add("Range1", 0, 0, 2, 2);
            ProtectedRange range1 = allowRanges[index1];
            range1.Password = "123";

            // Ajouter la deuxième plage protégée
            int index2 = allowRanges.Add("Range2", 3, 3, 5, 5);
            ProtectedRange range2 = allowRanges[index2];
            range2.Password = "456";

            // Afficher les informations CellArea pour les deux plages
            Console.WriteLine("Protected Range 1:");
            Console.WriteLine($"Name: {range1.Name}");
            Console.WriteLine($"Area: {range1.CellArea.StartRow},{range1.CellArea.StartColumn} to {range1.CellArea.EndRow},{range1.CellArea.EndColumn}");

            Console.WriteLine("\nProtected Range 2:");
            Console.WriteLine($"Name: {range2.Name}");
            Console.WriteLine($"Area: {range2.CellArea.StartRow},{range2.CellArea.StartColumn} to {range2.CellArea.EndRow},{range2.CellArea.EndColumn}");

            // Enregistrez le classeur
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



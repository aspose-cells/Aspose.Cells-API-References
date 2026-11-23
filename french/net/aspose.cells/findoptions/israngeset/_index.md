---
title: "FindOptions.IsRangeSet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FindOptions. Indique si la plage recherchée est définie"
type: docs
url: /fr/net/aspose.cells/findoptions/israngeset/
---
## FindOptions.IsRangeSet property

Indique si la plage recherchée est définie.

```csharp
public bool IsRangeSet { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertyIsRangeSetDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplissez quelques données
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Date");
            worksheet.Cells["B2"].PutValue("Elderberry");
            worksheet.Cells["B3"].PutValue("Fig");

            // Créer une instance de FindOptions
            FindOptions findOptions = new FindOptions();

            // Vérifiez la valeur initiale de IsRangeSet (devrait être false)
            Console.WriteLine("Initial IsRangeSet value: " + findOptions.IsRangeSet);

            // Définir une plage de recherche
            CellArea searchRange = new CellArea();
            searchRange.StartRow = 0;
            searchRange.StartColumn = 0;
            searchRange.EndRow = 2;
            searchRange.EndColumn = 0; // Column A only
            findOptions.SetRange(searchRange);

            // Vérifiez IsRangeSet après avoir défini la plage (devrait être true)
            Console.WriteLine("After SetRange, IsRangeSet value: " + findOptions.IsRangeSet);

            // Effectuer une opération de recherche dans la plage spécifiée
            Cell foundCell = worksheet.Cells.Find("Banana", null, findOptions);
            Console.WriteLine("Found 'Banana' at: " + foundCell?.Name);

            // Essayez de trouver quelque chose en dehors de la plage (ne devrait pas être trouvé)
            foundCell = worksheet.Cells.Find("Fig", null, findOptions);
            Console.WriteLine("Found 'Fig' at: " + foundCell?.Name); // Should be null

            // Enregistrez le classeur
            workbook.Save("PropertyIsRangeSetDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



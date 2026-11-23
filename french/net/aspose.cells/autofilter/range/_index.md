---
title: "AutoFilter.Range"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AutoFilter. Représente la plage à laquelle le filtre automatique spécifié s'applique"
type: docs
url: /fr/net/aspose.cells/autofilter/range/
---
## AutoFilter.Range property

Représente la plage à laquelle le AutoFilter spécifié s'applique.

```csharp
public string Range { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["A5"].PutValue("Item4");

            // Appliquer le filtre automatique à la plage A1:A5
            sheet.AutoFilter.Range = "A1:A5";

            // Afficher la plage du filtre automatique
            Console.WriteLine("AutoFilter Range: " + sheet.AutoFilter.Range);

            // Enregistrez le classeur
            workbook.Save("AutoFilterRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



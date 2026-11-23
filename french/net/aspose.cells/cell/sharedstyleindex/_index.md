---
title: "Cell.SharedStyleIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient l'index du style partagé de la cellule dans le pool de styles"
type: docs
url: /fr/net/aspose.cells/cell/sharedstyleindex/
---
## Cell.SharedStyleIndex property

Obtient l'index du style partagé de la cellule dans le pool de styles.

```csharp
public int SharedStyleIndex { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertySharedStyleIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un style et définir certaines propriétés
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;

            // Appliquer le style à la cellule A1
            worksheet.Cells["A1"].SetStyle(style);

            // Obtenir l'index du style partagé de la cellule A1
            int sharedStyleIndex = worksheet.Cells["A1"].SharedStyleIndex;

            // Récupérer le style du pool de styles en utilisant l'index
            Style retrievedStyle = workbook.GetStyleInPool(sharedStyleIndex);

            // Afficher les informations du style pour vérifier
            Console.WriteLine("Font Name: " + retrievedStyle.Font.Name);
            Console.WriteLine("Font Size: " + retrievedStyle.Font.Size);
            Console.WriteLine("Is Bold: " + retrievedStyle.Font.IsBold);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



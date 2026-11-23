---
title: "Cell.DateTimeValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient la valeur DateTime contenue dans la cellule"
type: docs
url: /fr/net/aspose.cells/cell/datetimevalue/
---
## Cell.DateTimeValue property

Obtient la valeur DateTime contenue dans la cellule.

```csharp
public DateTime DateTimeValue { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDateTimeValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir une valeur DateTime dans la cellule A1
            DateTime testDate = new DateTime(2023, 12, 25);
            cells["A1"].PutValue(testDate);

            // Formater la cellule pour afficher la date
            Style style = cells["A1"].GetStyle();
            style.Custom = "yyyy-MM-dd";
            cells["A1"].SetStyle(style);

            // Récupérer et vérifier le DateTimeValue
            DateTime retrievedDate = cells["A1"].DateTimeValue;
            Console.WriteLine("Original DateTime: " + testDate.ToString("yyyy-MM-dd"));
            Console.WriteLine("Retrieved DateTime: " + retrievedDate.ToString("yyyy-MM-dd"));

            // Définir une autre valeur DateTime dans la cellule B1
            DateTime anotherDate = new DateTime(2024, 1, 1);
            cells["B1"].PutValue(anotherDate);

            // Afficher le DateTimeValue depuis B1
            Console.WriteLine("B1 DateTime: " + cells["B1"].DateTimeValue.ToString("yyyy-MM-dd"));
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



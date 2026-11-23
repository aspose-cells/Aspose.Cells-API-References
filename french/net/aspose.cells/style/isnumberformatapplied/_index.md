---
title: "Style.IsNumberFormatApplied"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Indique si le formatage numérique doit être appliqué"
type: docs
url: /fr/net/aspose.cells/style/isnumberformatapplied/
---
## Style.IsNumberFormatApplied property

Indique si le formatage des nombres doit être appliqué.

```csharp
public bool IsNumberFormatApplied { get; set; }
```

### Remarques

Uniquement pour le style nommé.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsNumberFormatAppliedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer un style avec un format numérique
            Style style = workbook.CreateStyle();
            style.Number = 14; // Format as "m/d/yyyy"
            style.IsNumberFormatApplied = true;
            
            // Appliquer le style à une cellule
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Vérifier que le format numérique est appliqué
            Console.WriteLine("IsNumberFormatApplied: " + style.IsNumberFormatApplied);
            Console.WriteLine("Cell value format: " + cell.GetDisplayStyle().Number);
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



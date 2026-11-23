---
title: "Cell.DisplayStringValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient la valeur de chaîne formatée de cette cellule selon le style d'affichage de la cellule"
type: docs
url: /fr/net/aspose.cells/cell/displaystringvalue/
---
## Cell.DisplayStringValue property

Obtient la valeur chaîne formatée de cette cellule selon le style d'affichage de la cellule.

```csharp
public string DisplayStringValue { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDisplayStringValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cell cell = sheet.Cells[0, 0];
            
            // Premier exemple
            Style style = cell.GetStyle();
            style.Custom = "# ##/##\\\"";
            cell.SetStyle(style);
            cell.PutValue(3);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: 3"
            
            // Deuxième exemple
            style.Custom = "\"a\"#\"b\" \"c\"##\"d\"/\"e\"##";
            cell.SetStyle(style);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3
            
            // Troisième exemple
            style.Custom = "\"a\"#\"b\" \"c\"##\"d\"/\"e\"##\"f\"";
            cell.SetStyle(style);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3f
            
            // Quatrième exemple avec une valeur décimale
            cell.PutValue(1.234);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a1b c11d/e47f
            
            // Cinquième exemple avec un format modifié
            style.Custom = "\"a\"#\"b\"\"c\"##\"d\"/\"e\"##\"f\"";
            cell.SetStyle(style);
            cell.PutValue(3);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3f
            
            // Sixième exemple avec une valeur décimale
            cell.PutValue(1.234);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a1bc11d/e47f
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Style.ToJson"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Style. Convertit Style en données de structure JSON"
type: docs
url: /fr/net/aspose.cells/style/tojson/
---
## Style.ToJson method

Convertir [`Style`](../) en données de structure JSON.

```csharp
public string ToJson()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodToJsonDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer et appliquer un style à la cellule B4
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Yellow;
            cells["B4"].SetStyle(style);

            // Convertir le style en JSON
            string styleJson = style.ToJson();
            Console.WriteLine("Style JSON:");
            Console.WriteLine(styleJson);

            // Définissez la formule dans la cellule B6
            cells["B6"].Formula = "=A1";

            // Convertir la cellule en JSON
            string cellJson = cells["B6"].ToJson();
            Console.WriteLine("\nCell JSON:");
            Console.WriteLine(cellJson);
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



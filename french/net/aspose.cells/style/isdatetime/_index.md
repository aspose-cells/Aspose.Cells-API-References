---
title: "Style.IsDateTime"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Indique si le format numérique est un format de date"
type: docs
url: /fr/net/aspose.cells/style/isdatetime/
---
## Style.IsDateTime property

Indique si le format de nombre est un format de date.

```csharp
public bool IsDateTime { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsDateTimeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Définir une valeur numérique
            cells["A1"].PutValue(1230);
            
            // Obtenir et modifier le style de la cellule
            Style style = cells["A1"].GetStyle();
            
            // Définir au format date (15 est le format de date intégré)
            style.Number = 15;
            Console.WriteLine("IsDateTime after setting Number=15: " + style.IsDateTime);
            
            // Définir un format de date personnalisé
            style.Custom = "yyyy-mm-dd";
            Console.WriteLine("IsDateTime after setting custom date format: " + style.IsDateTime);
            
            // Appliquer le style modifié à la cellule
            cells["A1"].SetStyle(style);
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



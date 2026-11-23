---
title: "Style.Custom"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Représente la chaîne de format numérique personnalisé de cet objet style. Si le format numérique personnalisé n'est pas défini, par exemple le format numérique intégré sera renvoyé"
type: docs
url: /fr/net/aspose.cells/style/custom/
---
## Style.Custom property

Représente la chaîne de format numérique personnalisé de cet objet style. Si le format numérique personnalisé n'est pas défini (par exemple, le format numérique est intégré), "" sera retourné.

```csharp
public string Custom { get; set; }
```

### Remarques

La chaîne personnalisée renvoyée est indépendante de la culture.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyCustomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer et appliquer un format de date personnalisé
            Style style = workbook.CreateStyle();
            style.Custom = "d-mmm-yy";
            
            cells["A1"].PutValue(new DateTime(2023, 10, 15));
            cells["A1"].SetStyle(style);

            // Afficher la valeur formatée
            Console.WriteLine("Formatted value: " + cells["A1"].StringValue);
            
            // Enregistrez le classeur
            workbook.Save("StylePropertyCustomDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



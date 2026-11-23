---
title: "Style.IsPercent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Indique si le format numérique est un format pourcentage"
type: docs
url: /fr/net/aspose.cells/style/ispercent/
---
## Style.IsPercent property

Indique si le format de nombre est un format de pourcentage.

```csharp
public bool IsPercent { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StylePropertyIsPercentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accédez à la cellule A1 et définissez sa valeur
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(0.5);
            
            // Obtenir le style de la cellule
            Style style = cell.GetStyle();
            
            // Affichez la valeur actuelle de IsPercent
            Console.WriteLine("Current IsPercent value: " + style.IsPercent);
            
            // Définissez le format numérique en pourcentage (cela définira automatiquement IsPercent sur true)
            style.Number = 10; // 10 is the built-in percentage format in Excel
            
            // Appliquez le style à la cellule
            cell.SetStyle(style);
            
            // Vérifier que IsPercent est maintenant vrai
            Console.WriteLine("After setting percentage format, IsPercent value: " + style.IsPercent);
            
            // Créer une autre cellule avec un format différent
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue(0.75);
            Style style2 = cell2.GetStyle();
            style2.Number = 3; // 3 is the built-in number format (not percentage)
            cell2.SetStyle(style2);
            
            // Vérifier que IsPercent est faux pour un format non pourcentage
            Console.WriteLine("For non-percentage format, IsPercent value: " + style2.IsPercent);
            
            // Enregistrez le classeur
            workbook.Save("StylePropertyIsPercentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "SmartTagCollection.Row"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SmartTagCollection. Obtient la ligne des smart tags de la cellule"
type: docs
url: /fr/net/aspose.cells.markup/smarttagcollection/row/
---
## SmartTagCollection.Row property

Obtient la ligne des smart tags de la cellule.

```csharp
public int Row { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un smart tag à la cellule A1 (ligne 0, colonne 0)
            worksheet.Cells["A1"].PutValue("Sample with SmartTag");
            int index = worksheet.SmartTagSetting.Add("A1");
            
            // Obtenez la SmartTagCollection pour la cellule A1
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // Affichez la ligne de la cellule contenant ces smart tags
            Console.WriteLine("SmartTags are located at row: " + smartTags.Row);

            // Remarque : la propriété Row est en lecture seule, nous ne pouvons donc pas la définir
            // smartTags.Row = 5; // Cela provoquerait une erreur de compilation

            // Ajoutez un autre smart tag à la cellule B3 (ligne 2, colonne 1) pour démontrer une ligne différente
            worksheet.Cells["B3"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("B3");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at row: " + smartTags2.Row);

            // Enregistrez le classeur
            workbook.Save("SmartTagRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)



---
title: "SmartTagCollection.Column"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SmartTagCollection. Obtient la colonne des smart tags de la cellule"
type: docs
url: /fr/net/aspose.cells.markup/smarttagcollection/column/
---
## SmartTagCollection.Column property

Obtient la colonne des smart tags de la cellule.

```csharp
public int Column { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un smart tag à la cellule C5 (ligne 4, colonne 2)
            worksheet.Cells["C5"].PutValue("SmartTag Demo");
            int index = worksheet.SmartTagSetting.Add("C5");
            
            // Obtenez la SmartTagCollection pour la cellule C5
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // Affichez la colonne de la cellule contenant ces smart tags
            Console.WriteLine("SmartTags are located at column: " + smartTags.Column);

            // Ajoutez un autre smart tag à la cellule E2 (ligne 1, colonne 4) pour démontrer une colonne différente
            worksheet.Cells["E2"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("E2");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at column: " + smartTags2.Column);

            // Enregistrez le classeur
            workbook.Save("SmartTagColumnDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)



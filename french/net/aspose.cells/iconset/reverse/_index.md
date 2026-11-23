---
title: "IconSet.Reverse"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété IconSet. Obtenir ou définir le drapeau indiquant s'il faut inverser l'ordre par défaut des icônes dans cet ensemble d'icônes. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/iconset/reverse/
---
## IconSet.Reverse property

Obtenir ou définir le drapeau indiquant s'il faut inverser l'ordre par défaut des icônes dans cet ensemble d'icônes. La valeur par défaut est false.

```csharp
public bool Reverse { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyReverseDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Ajouter une mise en forme conditionnelle
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection cf = cfs[index];
            
            // Définir la plage
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            cf.AddArea(area);

            // Créer une mise en forme conditionnelle d'ensemble d'icônes
            cf.AddCondition(FormatConditionType.IconSet);
            IconSet iconSet = cf[0].IconSet;
            
            // Configurer l'ensemble d'icônes
            iconSet.Type = IconSetType.Arrows3;
            iconSet.ShowValue = true;
            
            // Démontrer la propriété Reverse
            Console.WriteLine("Original IconSet Reverse value: " + iconSet.Reverse);
            iconSet.Reverse = true;
            Console.WriteLine("Modified IconSet Reverse value: " + iconSet.Reverse);

            // Enregistrez le classeur
            workbook.Save("IconSetPropertyReverseDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



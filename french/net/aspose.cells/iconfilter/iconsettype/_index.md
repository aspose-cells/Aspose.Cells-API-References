---
title: "IconFilter.IconSetType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété IconFilter. Obtient et définit quel jeu d'icônes est utilisé pour ce critère de filtre"
type: docs
url: /fr/net/aspose.cells/iconfilter/iconsettype/
---
## IconFilter.IconSetType property

Obtient et définit quel jeu d'icônes est utilisé pour ce critère de filtre.

```csharp
public IconSetType IconSetType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconFilterPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplissez des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Créez un filtre automatique
            worksheet.AutoFilter.Range = "A1:A10";
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            filterColumn.FilterType = FilterType.IconFilter;

            // Obtenez le filtre d'icône
            IconFilter iconFilter = (IconFilter)filterColumn.Filter;

            // Afficher le IconSetType actuel (la valeur par défaut est None)
            Console.WriteLine("Current IconSetType: " + iconFilter.IconSetType);

            // Définir le jeu d'icônes à 3 flèches
            iconFilter.IconSetType = IconSetType.Arrows3;
            iconFilter.IconId = 1; // Show only middle arrow

            // Appliquer le formatage conditionnel pour visualiser les icônes
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
            int conditionIndex = formatConditionCollection.AddCondition(FormatConditionType.IconSet);
            FormatCondition formatCondition = formatConditionCollection[conditionIndex];
            formatCondition.IconSet.Type = IconSetType.Arrows3;
            
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            formatConditionCollection.AddArea(area);

            // Passer au jeu d'icônes feux tricolores
            iconFilter.IconSetType = IconSetType.TrafficLights31;
            iconFilter.IconId = 2; // Show only green light

            // Enregistrer le résultat
            workbook.Save("PropertyIconSetTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [IconSetType](../../iconsettype/)
* class [IconFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



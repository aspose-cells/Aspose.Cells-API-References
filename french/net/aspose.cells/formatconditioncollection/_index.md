---
title: "Classe FormatConditionCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.FormatConditionCollection class. Représente le formatage conditionnel. Les FormatConditions peuvent contenir jusqu'à trois formats conditionnels"
type: docs
url: /fr/net/aspose.cells/formatconditioncollection/
---
## FormatConditionCollection class

Représente la mise en forme conditionnelle. Les FormatConditions peuvent contenir jusqu'à trois formats conditionnels.

```csharp
public class FormatConditionCollection
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.cells/formatconditioncollection/count/) { get; } | Obtient le nombre de conditions. |
| [Item](../../aspose.cells/formatconditioncollection/item/) { get; } | Obtient la condition de formatage par index. |
| [RangeCount](../../aspose.cells/formatconditioncollection/rangecount/) { get; } | Obtient le nombre de plages formatées conditionnellement. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells/formatconditioncollection/add/)(CellArea, FormatConditionType, OperatorType, string, string) | Ajoute une condition de formatage et la plage de cellules affectée aux FormatConditions. Les FormatConditions peuvent contenir jusqu'à trois formats conditionnels. Les références aux autres feuilles ne sont pas autorisées dans les formules du formatage conditionnel. |
| [AddArea](../../aspose.cells/formatconditioncollection/addarea/)(CellArea) | Ajoute une plage de cellules formatée conditionnellement. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition)(FormatConditionType) | Ajouter une condition de format. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition_1)(FormatConditionType, OperatorType, string, string) | Ajoute une condition de formatage. |
| [GetCellArea](../../aspose.cells/formatconditioncollection/getcellarea/)(int) | Obtient la plage de cellules formatée conditionnellement par index. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea_1)(int) | Supprime la plage de cellules formatée conditionnellement par index. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea)(int, int, int, int) | Supprimer le formatage conditionnel dans la plage. |
| [RemoveCondition](../../aspose.cells/formatconditioncollection/removecondition/)(int) | Supprime la condition de formatage par index. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionDemo
    {
        public static void FormatConditionCollectionExample()
        {
            // Créez un nouveau classeur
            Workbook workbook = new Workbook();

            // Obtenir la première feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoute une mise en forme conditionnelle vide
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Définit la plage de mise en forme conditionnelle
            CellArea ca = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);
            ca = new CellArea { StartRow = 1, EndRow = 1, StartColumn = 1, EndColumn = 1 };
            fcs.AddArea(ca);

            // Ajoute des conditions
            int conditionIndex1 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

            // Définit la couleur d'arrière-plan
            FormatCondition fc1 = fcs[conditionIndex1];
            fc1.Style.BackgroundColor = System.Drawing.Color.Red;

            // Enregistrement du fichier Excel
            workbook.Save("FormatConditionCollectionExample.xlsx");
            workbook.Save("FormatConditionCollectionExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



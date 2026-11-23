---
title: "ConditionalFormattingCollection.Copy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ConditionalFormattingCollection. Copie la mise en forme conditionnelle"
type: docs
url: /fr/net/aspose.cells/conditionalformattingcollection/copy/
---
## ConditionalFormattingCollection.Copy method

Copie le formatage conditionnel.

```csharp
public void Copy(ConditionalFormattingCollection cfs)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cfs | ConditionalFormattingCollection | La mise en forme conditionnelle |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingCollectionMethodCopyWithConditionalFormattingCollectioDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // Créez un classeur source avec une mise en forme conditionnelle
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];

            // Ajoutez une mise en forme conditionnelle d'exemple à la feuille source
            int index = sourceSheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sourceSheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Créez et appliquez un style à la condition de format
            Style style = sourceWorkbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Red;
            FormatCondition fc = fcc[0];
            fc.Style = style;

            // Appliquer à une plage
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 5;
            area.StartColumn = 0;
            area.EndColumn = 5;
            fcc.AddArea(area);

            // Copiez la mise en forme conditionnelle de la source vers la destination
            destSheet.ConditionalFormattings.Copy(sourceSheet.ConditionalFormattings);

            // Enregistrez le classeur
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



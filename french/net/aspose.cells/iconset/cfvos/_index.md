---
title: "IconSet.Cfvos"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété IconSet. Obtenir l'instance CFValueObjects"
type: docs
url: /fr/net/aspose.cells/iconset/cfvos/
---
## IconSet.Cfvos property

Obtenir l'instance CFValueObjects.

```csharp
public ConditionalFormattingValueCollection Cfvos { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetPropertyCfvosDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            try
            {
                // Ajouter une mise en forme conditionnelle
                int cfIndex = worksheet.ConditionalFormattings.Add();
                FormatConditionCollection fcs = worksheet.ConditionalFormattings[cfIndex];

                // Définir la plage pour la mise en forme conditionnelle
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 9;
                area.EndColumn = 0;
                fcs.AddArea(area);

                // Ajouter une condition d'ensemble d'icônes
                int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcs[conditionIndex];

                // Définir le type d'ensemble d'icônes
                condition.IconSet.Type = IconSetType.TrafficLights31;

                // Accéder à la propriété Cfvos (lecture seule)
                ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

                // Afficher les informations sur la collection Cfvos
                Console.WriteLine("Number of CFValueObjects in the collection: " + cfvos.Count);

                // Parcourir la collection et afficher chaque valeur
                for (int i = 0; i < cfvos.Count; i++)
                {
                    ConditionalFormattingValue cfValue = cfvos[i];
                    Console.WriteLine($"CFValue {i + 1}: Type = {cfValue.Type}, Value = {cfValue.Value}");
                }

                // Enregistrez le classeur
                workbook.Save("IconSetCfvosDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon set conditional formatting.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ConditionalFormattingValueCollection](../../conditionalformattingvaluecollection/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



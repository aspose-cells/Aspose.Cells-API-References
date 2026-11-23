---
title: "ConditionalFormattingValue.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ConditionalFormattingValue. Obtenez ou définissez la valeur de cet objet de valeur de mise en forme conditionnelle. Elle doit être utilisée en conjonction avec Type"
type: docs
url: /fr/net/aspose.cells/conditionalformattingvalue/value/
---
## ConditionalFormattingValue.Value property

Obtenez ou définissez la valeur de cet objet de valeur de mise en forme conditionnelle. Elle doit être utilisée conjointement avec Type.

```csharp
public object Value { get; set; }
```

### Remarques

Si la valeur est une chaîne et commence par "=", elle sera traitée comme une formule, sinon nous la traiterons comme une valeur simple.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Ajouter une mise en forme conditionnelle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Créer une mise en forme conditionnelle d'ensemble d'icônes
            int conditionIndex = fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcc[conditionIndex];
            condition.IconSet.Type = IconSetType.Arrows3;

            // Obtenez les objets de valeur de mise en forme conditionnelle
            ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

            // Définissez les valeurs pour les icônes
            cfvos[0].Type = FormatConditionValueType.Min;
            cfvos[0].Value = 0;
            
            cfvos[1].Type = FormatConditionValueType.Percent;
            cfvos[1].Value = 33;
            
            cfvos[2].Type = FormatConditionValueType.Percent;
            cfvos[2].Value = 67;

            // Démontrez l'utilisation de la propriété Value
            Console.WriteLine("First icon value: " + cfvos[0].Value);
            Console.WriteLine("Second icon value: " + cfvos[1].Value);
            Console.WriteLine("Third icon value: " + cfvos[2].Value);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "ConditionalFormattingValue.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ConditionalFormattingValue. Obtenez ou définissez le type de cet objet de valeur de mise en forme conditionnelle. Définir le type sur FormatConditionValueType.Min ou FormatConditionValueType.Max définira automatiquement Value à null"
type: docs
url: /fr/net/aspose.cells/conditionalformattingvalue/type/
---
## ConditionalFormattingValue.Type property

Obtenez ou définissez le type de cet objet de valeur de mise en forme conditionnelle. Définir le type sur FormatConditionValueType.Min ou FormatConditionValueType.Max définira automatiquement "Value" à null.

```csharp
public FormatConditionValueType Type { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValuePropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                Worksheet ws = workbook.Worksheets[0];

                // Ajoutez des données d'exemple (nécessaires pour que la mise en forme conditionnelle existe)
                ws.Cells["A1"].PutValue(10);
                ws.Cells["A2"].PutValue(20);
                ws.Cells["A3"].PutValue(30);

                // Créez une collection de mise en forme conditionnelle et ajoutez une condition IconSet
                int cfIndex = ws.ConditionalFormattings.Add();
                FormatConditionCollection fcc = ws.ConditionalFormattings[cfIndex];

                int condIdx = fcc.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcc[condIdx];
                condition.IconSet.Type = IconSetType.Arrows3; // any valid icon set type

                // Obtenez une instance de ConditionalFormattingValue à partir de la collection IconSet
                ConditionalFormattingValue cfv = condition.IconSet.Cfvos[0];

                // Définissez le Type sur Percent et attribuez une valeur correspondante
                cfv.Type = FormatConditionValueType.Percent;
                cfv.Value = 25; // 25%

                // Lisez et affichez le Type et la Value
                Console.WriteLine("After setting Type to Percent:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + cfv.Value);

                // Changez le Type en Min – selon la documentation, cela annulera la Value
                cfv.Type = FormatConditionValueType.Min;

                // Lisez et affichez à nouveau le Type et la Value
                Console.WriteLine("\nAfter setting Type to Min:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + (cfv.Value == null ? "null" : cfv.Value.ToString()));

                // Enregistrez le classeur (la mise en forme conditionnelle fait partie de la feuille)
                workbook.Save("ConditionalFormattingValueTypeDemo.xlsx");
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

* enum [FormatConditionValueType](../../formatconditionvaluetype/)
* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "FormatCondition.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormatCondition. Obtient et définit le type du format conditionnel"
type: docs
url: /fr/net/aspose.cells/formatcondition/type/
---
## FormatCondition.Type property

Obtient et définit si le type de mise en forme conditionnelle est activé.

```csharp
public FormatConditionType Type { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Créer une mise en forme conditionnelle
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // Ajouter une condition de format avec le type d'expression (paramètres corrigés)
            int conditionIndex = fcs.AddCondition(FormatConditionType.Expression, OperatorType.None, "=A1>5", null);
            FormatCondition fc = fcs[conditionIndex];
            
            // Définir le style pour la condition
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // Démontrer l'utilisation de la propriété Type
            Console.WriteLine("Format Condition Type: " + fc.Type);
            
            // Enregistrez le classeur
            workbook.Save("FormatConditionPropertyTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



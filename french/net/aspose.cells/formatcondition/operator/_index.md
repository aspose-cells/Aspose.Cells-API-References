---
title: "FormatCondition.Operator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormatCondition. Obtient et définit le type d'opérateur de format conditionnel"
type: docs
url: /fr/net/aspose.cells/formatcondition/operator/
---
## FormatCondition.Operator property

Obtient et définit le type d'opérateur de mise en forme conditionnelle.

```csharp
public OperatorType Operator { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyOperatorDemo
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
            
            // Ajouter une mise en forme conditionnelle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Créer une plage de cellules
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            
            // Ajouter une condition
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "25");
            FormatCondition fc = fcc[conditionIndex];
            
            // Définir le style
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;
            
            // Démontrer l'utilisation de la propriété Operator
            Console.WriteLine("Operator Type: " + fc.Operator);
            if (fc.Operator == OperatorType.Between)
            {
                Console.WriteLine("Condition is set to BETWEEN values");
            }
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* enum [OperatorType](../../operatortype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



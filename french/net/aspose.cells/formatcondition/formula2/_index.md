---
title: "FormatCondition.Formula2"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormatCondition. Obtient et définit la valeur ou l'expression associée au formatage conditionnel"
type: docs
url: /fr/net/aspose.cells/formatcondition/formula2/
---
## FormatCondition.Formula2 property

Obtient et définit la valeur ou l'expression associée à la mise en forme conditionnelle.

```csharp
public string Formula2 { get; set; }
```

### Remarques

Veuillez ajouter toutes les zones avant de définir la formule. Pour définir la formule de cette condition, si la valeur d'entrée commence par '=', elle sera considérée comme une formule. Sinon, elle sera prise comme une valeur simple (texte, nombre, booléen). Pour une valeur texte commençant par '=', l'utilisateur peut la saisir comme formule au format : "=\"=...\"".

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula2Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une mise en forme conditionnelle
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[index];
            
            // Définir la plage de cellules
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            
            // Ajouter une condition de format avec Formula2
            formatConditions.Add(area, 
                FormatConditionType.CellValue, 
                OperatorType.Between, 
                "=\"abc def\"", 
                "=\"a\"&\"b\"");

            // Obtenir la condition de format
            FormatCondition formatCondition = formatConditions[0];

            // Afficher les formules
            Console.WriteLine("Formula1: " + formatCondition.Formula1);
            Console.WriteLine("Formula2: " + formatCondition.Formula2);

            // Enregistrez le classeur
            workbook.Save("FormatConditionFormula2Demo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



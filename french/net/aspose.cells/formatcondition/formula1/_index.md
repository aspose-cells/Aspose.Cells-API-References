---
title: "FormatCondition.Formula1"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormatCondition. Obtient et définit la valeur ou l'expression associée au formatage conditionnel"
type: docs
url: /fr/net/aspose.cells/formatcondition/formula1/
---
## FormatCondition.Formula1 property

Obtient et définit la valeur ou l'expression associée à la mise en forme conditionnelle.

```csharp
public string Formula1 { get; set; }
```

### Remarques

Veuillez ajouter toutes les zones avant de définir la formule. Pour définir la formule de cette condition, si la valeur d'entrée commence par '=', elle sera considérée comme une formule. Sinon, elle sera prise comme une valeur simple (texte, nombre, booléen). Pour une valeur texte commençant par '=', l'utilisateur peut la saisir comme formule au format : "=\"=...\"".

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula1Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["E1"].PutValue(50);
            
            // Ajouter une mise en forme conditionnelle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Définir la plage et le type de condition
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.LessOrEqual, "=$E$1<=100", null);
            
            // Accéder et afficher la propriété Formula1
            FormatCondition fc = fcc[0];
            Console.WriteLine("Formula1: " + fc.Formula1);
        }
    }
}
```

### Voir aussi

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Classe FormatCondition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.FormatCondition. Représente une condition de mise en forme conditionnelle"
type: docs
url: /fr/net/aspose.cells/formatcondition/
---
## FormatCondition class

Représente la condition de mise en forme conditionnelle.

```csharp
public class FormatCondition
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage/) { get; } | Obtenez l'instance "AboveAverage" de la mise en forme conditionnelle. La règle de l'instance par défaut met en surbrillance les cellules dont la valeur est supérieure à la moyenne de toutes les valeurs de la plage. Valide uniquement pour le type = AboveAverage. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale/) { get; } | Obtenez l'instance "ColorScale" de la mise en forme conditionnelle. L'instance par défaut est une échelle de couleurs "vert-jaune-rouge" 3ColorScale. Valide uniquement pour le type = ColorScale. |
| [DataBar](../../aspose.cells/formatcondition/databar/) { get; } | Obtenez l'instance "DataBar" de la mise en forme conditionnelle. La couleur de l'instance par défaut est bleue. Valide uniquement pour le type = DataBar. |
| [Formula1](../../aspose.cells/formatcondition/formula1/) { get; set; } | Obtient et définit la valeur ou l'expression associée à la mise en forme conditionnelle. |
| [Formula2](../../aspose.cells/formatcondition/formula2/) { get; set; } | Obtient et définit la valeur ou l'expression associée à la mise en forme conditionnelle. |
| [IconSet](../../aspose.cells/formatcondition/iconset/) { get; } | Obtenez l'instance "IconSet" de la mise en forme conditionnelle. Le type IconSetType de l'instance par défaut est TrafficLights31. Valide uniquement pour le type = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator/) { get; set; } | Obtient et définit le type d'opérateur de mise en forme conditionnelle. |
| [Priority](../../aspose.cells/formatcondition/priority/) { get; set; } | La priorité de cette règle de mise en forme conditionnelle. Cette valeur est utilisée pour déterminer quel format doit être évalué et rendu. Les valeurs numériques plus faibles ont une priorité plus élevée que les valeurs numériques plus élevées, où '1' représente la priorité la plus haute. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue/) { get; set; } | Vrai, aucune règle avec une priorité inférieure ne peut être appliquée au-dessus de cette règle, lorsque celle‑ci s'évalue à vrai. S'applique uniquement à Excel 2007 ; |
| [Style](../../aspose.cells/formatcondition/style/) { get; set; } | Obtient ou définit le style des plages de cellules mises en forme conditionnelle. |
| [Text](../../aspose.cells/formatcondition/text/) { get; set; } | La valeur texte dans une règle de mise en forme conditionnelle "text contains". Valide uniquement pour les types = containsText, notContainsText, beginsWith et endsWith. La valeur par défaut est null. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod/) { get; set; } | La période de temps applicable dans une règle de mise en forme conditionnelle "date occurrin". Valide uniquement pour le type = timePeriod. La valeur par défaut est TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10/) { get; } | Obtenez l'instance "Top10" de la mise en forme conditionnelle. La règle de l'instance par défaut met en surbrillance les cellules dont les valeurs se situent dans le top 10. Valide uniquement pour le type = Top10. |
| [Type](../../aspose.cells/formatcondition/type/) { get; set; } | Obtient et définit si le type de mise en forme conditionnelle est activé. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1)(bool, bool) | Obtient la valeur ou l'expression associée à cette condition de format. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_2)(int, int) | Obtient la formule de la mise en forme conditionnelle de la cellule. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_1)(bool, bool, int, int) | Obtient la valeur ou l'expression de la mise en forme conditionnelle de la cellule. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2)(bool, bool) | Obtient la valeur ou l'expression associée à cette condition de format. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_2)(int, int) | Obtient la formule de la mise en forme conditionnelle de la cellule. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_1)(bool, bool, int, int) | Obtient la valeur ou l'expression de la mise en forme conditionnelle de la cellule. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1/)(string, bool, bool) | Définit la valeur ou l'expression associée à cette condition de format. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2/)(string, bool, bool) | Définit la valeur ou l'expression associée à cette condition de format. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas/)(string, string, bool, bool) | Définit la valeur ou l'expression associée à cette condition de format. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FormatConditionDemo
    {
        public static void FormatConditionExample()
        {
            // Créez un nouveau classeur.
            Workbook workbook = new Workbook();

            // Obtenez la première feuille de calcul.
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoute une mise en forme conditionnelle vide
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Définit la plage de mise en forme conditionnelle.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Ajoute une condition.
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            FormatCondition fc = fcs[conditionIndex];

            // Définition des propriétés
            fc.Formula1 = "=A2";
            fc.Formula2 = "100";
            fc.Operator = OperatorType.Between;
            fc.StopIfTrue = true;
            fc.Priority = 1;
            fc.Style.BackgroundColor = Color.Red;
            fc.Type = FormatConditionType.CellValue;

            // Démonstration d'autres propriétés
            fc.Text = "Sample Text";
            fc.TimePeriod = TimePeriodType.Today;

            // Enregistrement du fichier Excel
            workbook.Save("FormatConditionExample.xlsx");
            workbook.Save("FormatConditionExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



---
title: FormatCondition
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente la condition de mise en forme conditionnelle.
type: docs
weight: 3560
url: /fr/net/aspose.cells/formatcondition/
---
## FormatCondition class

Représente la condition de mise en forme conditionnelle.

```csharp
public class FormatCondition
```

## Propriétés

| Nom | La description |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage) { get; } | Obtenez l'instance "AboveAverage" de la mise en forme conditionnelle. La règle de l'instance par défaut met en évidence les cellules qui sont au-dessus de la moyenne pour toutes les valeurs de la plage. Valable uniquement pour le type = AboveAverage. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale) { get; } | Récupère l'instance "ColorScale" de la mise en forme conditionnelle. L'instance par défaut est une 3ColorScale "vert-jaune-rouge". Valable uniquement pour le type = ColorScale. |
| [DataBar](../../aspose.cells/formatcondition/databar) { get; } | Obtenir l'instance "DataBar" de la mise en forme conditionnelle. La couleur par défaut de l'instance est le bleu. Valide uniquement pour le type est DataBar. |
| [Formula1](../../aspose.cells/formatcondition/formula1) { get; set; } | Obtient et définit la valeur ou l'expression associée à la mise en forme conditionnelle. |
| [Formula2](../../aspose.cells/formatcondition/formula2) { get; set; } | Obtient et définit la valeur ou l'expression associée à la mise en forme conditionnelle. |
| [IconSet](../../aspose.cells/formatcondition/iconset) { get; } | Obtenir l'instance "IconSet" de la mise en forme conditionnelle. L'IconSetType de l'instance par défaut est TrafficLights31. Valable uniquement pour le type = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator) { get; set; } | Obtient et définit le type d'opérateur de format conditionnel. |
| [Priority](../../aspose.cells/formatcondition/priority) { get; set; } | La priorité de cette règle de mise en forme conditionnelle. Cette valeur est utilisée pour déterminer quel format doit être évalué et rendu. Les valeurs numériques inférieures ont une priorité plus élevée que les valeurs numériques supérieures, où '1' est la priorité la plus élevée. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue) { get; set; } | True, aucune règle avec une priorité inférieure ne peut être appliquée sur cette règle, lorsque cette règle est évaluée à true. S'applique uniquement à Excel 2007 ; |
| [Style](../../aspose.cells/formatcondition/style) { get; set; } | Obtient ou définit le style des plages de cellules formatées conditionnelles. |
| [Text](../../aspose.cells/formatcondition/text) { get; set; } | La valeur de texte dans une règle de mise en forme conditionnelle "le texte contient". Valide uniquement pour type = containsText, notContainsText, startsWith et endsWith. La valeur par défaut est null. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod) { get; set; } | La période applicable dans une règle de mise en forme conditionnelle "date survenant…". Valide uniquement pour type = timePeriod. La valeur par défaut est TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10) { get; } | Obtenir l'instance "Top10" de la mise en forme conditionnelle. La règle de l'instance par défaut met en surbrillance les cellules dont les valeurs se situent dans les 10 premières tranches. Valable uniquement pour le type Top10. |
| [Type](../../aspose.cells/formatcondition/type) { get; set; } | Obtient et définit si le format conditionnel Type. |

## Méthodes

| Nom | La description |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1)(bool, bool) | Obtient la valeur ou l'expression associée à cette condition de format. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_2)(int, int) | Obtient la formule de la mise en forme conditionnelle de la cellule. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_1)(bool, bool, int, int) | Obtient la valeur ou l'expression de la mise en forme conditionnelle de la cellule. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2)(bool, bool) | Obtient la valeur ou l'expression associée à cette condition de format. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_2)(int, int) | Obtient la formule de la mise en forme conditionnelle de la cellule. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_1)(bool, bool, int, int) | Obtient la valeur ou l'expression de la mise en forme conditionnelle de la cellule. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1)(string, bool, bool) | Définit la valeur ou l'expression associée à cette condition de format. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2)(string, bool, bool) | Définit la valeur ou l'expression associée à cette condition de format. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas)(string, string, bool, bool) | Définit la valeur ou l'expression associée à cette condition de format. |

### Exemples

```csharp

[C#]
//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
 
//Ajoute une mise en forme conditionnelle vide
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
 
// Définit la plage de format conditionnel.
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.AddArea(ca);
 
ca = new CellArea();
ca.StartRow = 1;
ca.EndRow = 1;
ca.StartColumn = 1;
ca.EndColumn = 1;
fcs.AddArea(ca);
 
//Ajoute une condition.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
 
//Ajoute une condition.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
 
// Définit la couleur d'arrière-plan.
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
 
//Enregistrement du fichier Excel
workbook.Save("output.xls");

[VB.NET]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()
Dim sheet As Worksheet = workbook.Worksheets(0)
 
' Ajoute une mise en forme conditionnelle vide
Dim index As Integer = sheet.ConditionalFormattings.Add()
Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)
 
'Définit la plage de format conditionnel.
Dim ca As CellArea = New CellArea()
ca.StartRow = 0
ca.EndRow = 0
ca.StartColumn = 0
ca.EndColumn = 0
fcs.AddArea(ca)
ca = New CellArea()
ca.StartRow = 1
ca.EndRow = 1
ca.StartColumn = 1
ca.EndColumn = 1
fcs.AddArea(ca)
 
'Ajoute un état.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100")
 
'Ajoute un état.
Dim conditionIndex2 As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100")
 
'Définit la couleur d'arrière-plan.
Dim fc As FormatCondition = fcs(conditionIndex)
fc.Style.BackgroundColor = Color.Red
 
'Enregistrement du fichier Excel
workbook.Save("output.xls")
```

### Voir également

* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

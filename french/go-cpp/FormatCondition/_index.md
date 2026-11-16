---
title: "FormatCondition Class"
linktitle: "FormatCondition"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "FormatCondition class. Encapsule l'objet qui représente formatcondition en Go."
type: docs
weight: 200
url: /fr/go-cpp/formatcondition/
---

## FormatCondition class

Représente une condition de mise en forme conditionnelle.

```go

type FormatCondition struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetFormula1_Bool_Bool](./getformula1_bool_bool/) | Obtient la valeur ou l'expression associée à cette condition de format. |
| [GetFormula2_Bool_Bool](./getformula2_bool_bool/) | Obtient la valeur ou l'expression associée à cette condition de format. |
| [GetFormula1_Bool_Bool_Int_Int](./getformula1_bool_bool_int_int/) | Obtient la valeur ou l'expression du format conditionnel de la cellule. |
| [GetFormula2_Bool_Bool_Int_Int](./getformula2_bool_bool_int_int/) | Obtient la valeur ou l'expression du format conditionnel de la cellule. |
| [SetFormulas](./setformulas/) | Définit la valeur ou l'expression associée à cette condition de format. |
| [SetFormula1_String_Bool_Bool](./setformula1_string_bool_bool/) | Définit la valeur ou l'expression associée à cette condition de format. |
| [SetFormula2_String_Bool_Bool](./setformula2_string_bool_bool/) | Définit la valeur ou l'expression associée à cette condition de format. |
| [GetFormula1](./getformula1/) | Obtient et définit la valeur ou l'expression associée au format conditionnel. |
| [SetFormula1_String](./setformula1_string/) | Obtient et définit la valeur ou l'expression associée au format conditionnel. |
| [GetFormula1_Int_Int](./getformula1_int_int/) | Obtient la formule du format conditionnel de la cellule. |
| [GetFormula2](./getformula2/) | Obtient et définit la valeur ou l'expression associée au format conditionnel. |
| [SetFormula2_String](./setformula2_string/) | Obtient et définit la valeur ou l'expression associée au format conditionnel. |
| [GetFormula2_Int_Int](./getformula2_int_int/) | Obtient la formule du format conditionnel de la cellule. |
| [GetOperator](./getoperator/) | Obtient et définit le type d'opérateur du format conditionnel. |
| [SetOperator](./setoperator/) | Obtient et définit le type d'opérateur du format conditionnel. |
| [GetStopIfTrue](./getstopiftrue/) | Vrai, aucune règle de priorité inférieure ne peut être appliquée à cette règle, lorsque cette règle s'évalue à vrai. Uniquement applicable à Excel 2007 ; |
| [SetStopIfTrue](./setstopiftrue/) | Vrai, aucune règle de priorité inférieure ne peut être appliquée à cette règle, lorsque cette règle s'évalue à vrai. Uniquement applicable à Excel 2007 ; |
| [GetPriority](./getpriority/) | La priorité de cette règle de format conditionnel. Cette valeur est utilisée pour déterminer quel format doit être évalué et rendu. Les valeurs numériques inférieures ont une priorité plus élevée que les valeurs numériques supérieures, où '1' est la priorité la plus élevée. |
| [SetPriority](./setpriority/) | La priorité de cette règle de format conditionnel. Cette valeur est utilisée pour déterminer quel format doit être évalué et rendu. Les valeurs numériques inférieures ont une priorité plus élevée que les valeurs numériques supérieures, où '1' est la priorité la plus élevée. |
| [GetStyle](./getstyle/) | Obtient ou définit le style des plages de cellules formatées conditionnellement. |
| [SetStyle](./setstyle/) | Obtient ou définit le style des plages de cellules formatées conditionnellement. |
| [GetType](./gettype/) | Obtient et définit le type de format conditionnel. |
| [SetType](./settype/) | Obtient et définit le type de format conditionnel. |
| [GetIconSet](./geticonset/) | Obtient l'instance "IconSet" du format conditionnel. Le type d'instance par défaut IconSetType est TrafficLights31. Valide uniquement pour le type = IconSet. |
| [GetDataBar](./getdatabar/) | Obtient l'instance "DataBar" du format conditionnel. La couleur de l'instance par défaut est bleue. Valide uniquement pour le type = DataBar. |
| [GetColorScale](./getcolorscale/) | Obtient l'instance "ColorScale" du format conditionnel. L'instance par défaut est une "green-yellow-red" 3ColorScale. Valide uniquement pour le type = ColorScale. |
| [GetTop10](./gettop10/) | Obtient l'instance "Top10" du format conditionnel. La règle de l'instance par défaut met en évidence les cellules dont les valeurs se situent dans le top 10. Valide uniquement pour le type = Top10. |
| [GetAboveAverage](./getaboveaverage/) | Obtient l'instance "AboveAverage" du format conditionnel. La règle de l'instance par défaut met en évidence les cellules qui sont au-dessus de la moyenne pour toutes les valeurs de la plage. Valide uniquement pour le type = AboveAverage. |
| [GetText](./gettext/) | La valeur texte dans une règle de format conditionnel "text contains". Valide uniquement pour les types = containsText, notContainsText, beginsWith et endsWith. La valeur par défaut est null. |
| [SetText](./settext/) | La valeur texte dans une règle de format conditionnel "text contains". Valide uniquement pour les types = containsText, notContainsText, beginsWith et endsWith. La valeur par défaut est null. |
| [GetTimePeriod](./gettimeperiod/) | La période applicable dans une règle de format conditionnel "date occurrin". Valide uniquement pour le type = timePeriod. La valeur par défaut est TimePeriodType.Today. |
| [SetTimePeriod](./settimeperiod/) | La période applicable dans une règle de format conditionnel "date occurrin". Valide uniquement pour le type = timePeriod. La valeur par défaut est TimePeriodType.Today. |

---
title: "Classe PivotGlobalizationSettings"
linktitle: "PivotGlobalizationSettings"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe PivotGlobalizationSettings. Encapsule l'objet qui représente pivotglobalizationsettings en Go."
type: docs
weight: 200
url: /fr/go-cpp/pivotglobalizationsettings/
---

## PivotGlobalizationSettings class

Représente les paramètres de mondialisation pour les tableaux croisés dynamiques.

```go

type PivotGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewPivotGlobalizationSettings](./newpivotglobalizationsettings/) | Constructeur par défaut. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetTextOfTotal](./gettextoftotal/) | Obtient le texte de l'étiquette "Total" dans le PivotTable. Vous devez remplacer cette méthode lorsque le PivotTable contient deux champs Pivot ou plus dans la zone de données. |
| [GetTextOfGrandTotal](./gettextofgrandtotal/) | Obtient le texte de l'étiquette "Grand Total" dans le PivotTable. |
| [GetTextOfMultipleItems](./gettextofmultipleitems/) | Obtient le texte de l'étiquette "(Multiple Items)" dans le PivotTable. |
| [GetTextOfAll](./gettextofall/) | Obtient le texte de l'étiquette "(All)" dans le PivotTable. |
| [GetTextOfProtectedName](./gettextofprotectedname/) | Obtient le texte pour le nom protégé spécifié. |
| [GetTextOfColumnLabels](./gettextofcolumnlabels/) | Obtient le texte de l'étiquette "Column Labels" dans le PivotTable. |
| [GetTextOfRowLabels](./gettextofrowlabels/) | Obtient le texte de l'étiquette "Row Labels" dans le PivotTable. |
| [GetTextOfEmptyData](./gettextofemptydata/) | Obtient le texte de l'étiquette "(blank)" dans le PivotTable. |
| [GetTextOfDataFieldHeader](./gettextofdatafieldheader/) | Obtient le texte de l'en-tête du champ de la zone de valeurs dans le PivotTable. |
| [GetShortTextOf12Months](./getshorttextof12months/) | Obtient toutes les chaînes formatées courtes des 12 mois. |
| [GetTextOf24Hours](./gettextof24hours/) | Obtient toutes les chaînes formatées localement des 24 heures. La valeur par défaut est 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM. |
| [GetTextOfOr](./gettextofor/) | Obtient toutes les chaînes formatées localement de "or". |
| [GetFormatOfDayGroup](./getformatofdaygroup/) | Obtient le format numérique du groupe de jour du pivot. Utilisé uniquement lors du regroupement du champ pivot par jours. La valeur par défaut est "d-MMM"; |
| [GetTextOf4Quaters](./gettextof4quaters/) | Obtient le texte local des 4 trimestres. |
| [GetTextOf4Quarters](./gettextof4quarters/) | Obtient le texte local des 4 trimestres. |
| [GetTextOfYears](./gettextofyears/) | Obtient le texte local de "Years". |
| [GetTextOfQuarters](./gettextofquarters/) | Obtenez le texte local de "Quarters". |
| [GetTextOfMonths](./gettextofmonths/) | Récupère le texte local de "Months". |
| [GetTextOfDays](./gettextofdays/) | Récupère le texte local de "Days". |
| [GetTextOfHours](./gettextofhours/) | Récupère le texte local de "Hours". |
| [GetTextOfMinutes](./gettextofminutes/) | Récupère le texte local de "Minutes". |
| [GetTextOfSeconds](./gettextofseconds/) | Récupère le texte local de "Seconds" |
| [GetTextOfRange](./gettextofrange/) | Récupère le texte local de "Range" |
| [GetTextOfAllPeriods](./gettextofallperiods/) | Récupère le texte local de "All Periods" |
| [GetTextOfSubTotal](./gettextofsubtotal/) | Récupère le texte du type PivotFieldSubtotalType dans le PivotTable. |
| [GetNameOfDataField](./getnameofdatafield/) | Récupère le nom d'affichage du champ pivot de données.Le format par défaut est "Sum Of Field". |

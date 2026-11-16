---
title: "Classe PivotArea"
linktitle: "PivotArea"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe PivotArea. Encapsule l'objet qui représente pivotarea en Go."
type: docs
weight: 200
url: /fr/go-cpp/pivotarea/
---

## PivotArea class

Présente la zone sélectionnée du tableau croisé dynamique.

```go

type PivotArea struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewPivotArea](./newpivotarea/) | Présente la zone sélectionnée du PivotTable. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetFilters](./getfilters/) | Obtient tous les filtres pour ce PivotArea. |
| [Select](./select/) | Sélectionnez la zone avec des filtres. |
| [SelectField_PivotFieldType_String](./selectfield_pivotfieldtype_string/) | Sélectionnez un champ dans la région comme zone. |
| [SelectField_PivotFieldType_PivotField](./selectfield_pivotfieldtype_pivotfield/) | Sélectionnez un champ dans la région comme zone. |
| [GetOnlyData](./getonlydata/) | Indique si seules les valeurs de données (dans la zone de données de la vue) pour une sélection d'éléments sont sélectionnées et n'inclut pas les libellés des éléments. |
| [SetOnlyData](./setonlydata/) | Indique si seules les valeurs de données (dans la zone de données de la vue) pour une sélection d'éléments sont sélectionnées et n'inclut pas les libellés des éléments. |
| [GetOnlyLabel](./getonlylabel/) | Indique si seuls les libellés de données pour une sélection d'éléments sont sélectionnés. |
| [SetOnlyLabel](./setonlylabel/) | Indique si seuls les libellés de données pour une sélection d'éléments sont sélectionnés. |
| [IsRowGrandIncluded](./isrowgrandincluded/) | Indique si le total général des lignes est inclus. |
| [SetIsRowGrandIncluded](./setisrowgrandincluded/) | Indique si le total général des lignes est inclus. |
| [IsColumnGrandIncluded](./iscolumngrandincluded/) | Indique si le total général des colonnes est inclus. |
| [SetIsColumnGrandIncluded](./setiscolumngrandincluded/) | Indique si le total général des colonnes est inclus. |
| [GetAxisType](./getaxistype/) | Obtient et définit la région du PivotTable à laquelle cette règle s'applique. |
| [SetAxisType](./setaxistype/) | Obtient et définit la région du PivotTable à laquelle cette règle s'applique. |
| [GetRuleType](./getruletype/) | Obtient et définit le type de règle de sélection. |
| [SetRuleType](./setruletype/) | Obtient et définit le type de règle de sélection. |
| [IsOutline](./isoutline/) | Indique si la règle se réfère à une zone en mode plan. |
| [SetIsOutline](./setisoutline/) | Indique si la règle se réfère à une zone en mode plan. |
| [GetCellAreas](./getcellareas/) | Obtient les zones de cellules de cette zone de tableau croisé dynamique. |

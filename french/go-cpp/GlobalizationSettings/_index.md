---
title: "GlobalizationSettings Classe"
linktitle: "GlobalizationSettings"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "GlobalizationSettings class. Encapsule l'objet qui représente globalizationsettings en Go."
type: docs
weight: 200
url: /fr/go-cpp/globalizationsettings/
---

## GlobalizationSettings class

Représente les paramètres de mondialisation.

```go

type GlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewGlobalizationSettings](./newglobalizationsettings/) | Constructeur par défaut. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetChartSettings](./getchartsettings/) | Obtient les paramètres de globalisation pour Chart. |
| [SetChartSettings](./setchartsettings/) | Définit les paramètres de globalisation pour Chart. |
| [GetPivotSettings](./getpivotsettings/) | Obtient les paramètres de globalisation pour pivot table. |
| [SetPivotSettings](./setpivotsettings/) | Définit les paramètres de globalisation pour pivot table. |
| [GetTotalName](./gettotalname/) | Obtient le nom total de la fonction. |
| [GetGrandTotalName](./getgrandtotalname/) | Obtient le nom du total général de la fonction. |
| [GetDefaultSheetName](./getdefaultsheetname/) | Obtient le nom de feuille par défaut pour l'ajout automatique de feuille de calcul. La valeur par défaut est "Sheet". |
| [GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | Obtient le nom du type des lignes de tableau qui composent l'en-tête du tableau. La valeur par défaut est "Headers", ainsi dans la formule "#Headers" représente l'en-tête du tableau. |
| [GetTableRowTypeOfData](./gettablerowtypeofdata/) | Obtient le nom du type des lignes de tableau qui composent la région de données du tableau référencé. La valeur par défaut est "Data", ainsi dans la formule "#Data" représente la région de données du tableau. |
| [GetTableRowTypeOfAll](./gettablerowtypeofall/) | Obtient le nom du type des lignes de tableau qui comprend toutes les lignes du tableau référencé. La valeur par défaut est "All", ainsi dans la formule "#All" représente toutes les lignes du tableau référencé. |
| [GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | Obtient le nom du type des lignes de tableau qui comprend la ligne totale du tableau référencé. La valeur par défaut est "Totals", ainsi dans la formule "#Totals" représente la ligne totale du tableau référencé. |
| [GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | Obtient le nom du type des lignes de tableau qui comprend la ligne actuelle du tableau référencé. La valeur par défaut est "This Row", ainsi dans la formule "#This Row" représente la ligne actuelle du tableau référencé. |
| [GetErrorValueString](./geterrorvaluestring/) | Obtient la chaîne d'affichage de la valeur d'erreur de la cellule |
| [GetBooleanValueString](./getbooleanvaluestring/) | Obtient la chaîne d'affichage de la valeur booléenne de la cellule |
| [GetLocalFunctionName](./getlocalfunctionname/) | Obtient le nom de fonction dépendant de la locale selon le nom de fonction standard fourni. |
| [GetStandardFunctionName](./getstandardfunctionname/) | Obtient le nom de fonction standard selon le nom de fonction dépendant de la locale fourni. |
| [GetLocalBuiltInName](./getlocalbuiltinname/) | Obtient le texte dépendant de la locale pour le Nom intégré selon le texte standard fourni. |
| [GetStandardBuiltInName](./getstandardbuiltinname/) | Obtient le texte standard du Nom intégré selon le texte dépendant de la locale fourni. |
| [GetListSeparator](./getlistseparator/) | Obtient le séparateur pour les listes, les paramètres de fonction, etc. |
| [GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | Obtient le séparateur pour les lignes dans les données de tableau dans la formule. |
| [GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | Obtient le séparateur pour les éléments dans les données de ligne du tableau dans la formule. |
| [GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | Obtient le nom de style de police anglais standard (Regular, Bold, Italic) pour l'en-tête/pied de page selon le nom de style de police de la locale donnée. |
| [GetCommentTitleName](./getcommenttitlename/) | Obtient le nom du titre de commentaire dépendant de la locale selon le type de titre de commentaire. |
| [Compare](./compare/) | Compare deux valeurs de chaîne selon certaines règles de collation. |

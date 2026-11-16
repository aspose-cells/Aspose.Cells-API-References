---
title: "Classe CalculationData"
linktitle: "CalculationData"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe CalculationData. Encapsule l'objet qui représente calculationdata en Go."
type: docs
weight: 200
url: /fr/go-cpp/calculationdata/
---

## CalculationData class

Représente les données requises lors du calcul d'une fonction, telles que le nom de la fonction, les paramètres, etc.

```go

type CalculationData struct  {
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
| [GetCalculatedValue](./getcalculatedvalue/) | Obtient ou définit la valeur calculée pour cette fonction. |
| [SetCalculatedValue](./setcalculatedvalue/) | Obtient ou définit la valeur calculée pour cette fonction. |
| [GetWorkbook](./getworkbook/) | Obtient l'objet Workbook où se trouve la fonction. |
| [GetWorksheet](./getworksheet/) | Obtient l'objet Worksheet où se trouve la fonction. |
| [GetCellRow](./getcellrow/) | Obtient l'index de ligne de la cellule où se trouve la fonction. |
| [GetCellColumn](./getcellcolumn/) | Obtient l'index de colonne de la cellule où se trouve la fonction. |
| [GetCell](./getcell/) | Obtient l'objet Cell où se trouve la fonction. |
| [GetFunctionName](./getfunctionname/) | Obtient le nom de la fonction à calculer. |
| [GetParamCount](./getparamcount/) | Obtient le nombre de paramètres |
| [GetParamValue](./getparamvalue/) | Obtient l'objet valeur représentée du paramètre à un index donné. |
| [GetParamValueInArrayMode](./getparamvalueinarraymode/) | Obtient la ou les valeurs du paramètre à un index donné. Si le paramètre est une sorte d'expression qui doit être calculée, alors elle sera calculée en mode tableau. |
| [GetParamText](./getparamtext/) | Obtient le texte littéral du paramètre à l'index donné. |

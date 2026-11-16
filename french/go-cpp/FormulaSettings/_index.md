---
title: "Classe FormulaSettings"
linktitle: "FormulaSettings"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe FormulaSettings. Encapsule l'objet qui représente formulasettings en Go."
type: docs
weight: 200
url: /fr/go-cpp/formulasettings/
---

## FormulaSettings class

Paramètres des formules et du calcul.

```go

type FormulaSettings struct  {
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
| [GetCalculateOnOpen](./getcalculateonopen/) | Indique si l'application doit effectuer un calcul complet lorsque le classeur est ouvert. |
| [SetCalculateOnOpen](./setcalculateonopen/) | Indique si l'application doit effectuer un calcul complet lorsque le classeur est ouvert. |
| [GetCalculateOnSave](./getcalculateonsave/) | Indique s'il faut recalculer le classeur avant d'enregistrer le document, en mode de calcul manuel. |
| [SetCalculateOnSave](./setcalculateonsave/) | Indique s'il faut recalculer le classeur avant d'enregistrer le document, en mode de calcul manuel. |
| [GetForceFullCalculation](./getforcefullcalculation/) | Indique s'il calcule toutes les formules à chaque fois lorsqu'un calcul est déclenché. |
| [SetForceFullCalculation](./setforcefullcalculation/) | Indique s'il calcule toutes les formules à chaque fois lorsqu'un calcul est déclenché. |
| [GetCalculationMode](./getcalculationmode/) | Obtient ou définit le mode de calcul du classeur dans MS Excel. |
| [SetCalculationMode](./setcalculationmode/) | Obtient ou définit le mode de calcul du classeur dans MS Excel. |
| [GetCalculationId](./getcalculationid/) | Spécifie la version du moteur de calcul utilisé pour calculer les valeurs du classeur. |
| [SetCalculationId](./setcalculationid/) | Spécifie la version du moteur de calcul utilisé pour calculer les valeurs du classeur. |
| [GetEnableIterativeCalculation](./getenableiterativecalculation/) | Indique s'il faut activer le calcul itératif pour résoudre les références circulaires. |
| [SetEnableIterativeCalculation](./setenableiterativecalculation/) | Indique s'il faut activer le calcul itératif pour résoudre les références circulaires. |
| [GetMaxIteration](./getmaxiteration/) | Le nombre maximal d'itérations pour résoudre une référence circulaire. |
| [SetMaxIteration](./setmaxiteration/) | Le nombre maximal d'itérations pour résoudre une référence circulaire. |
| [GetMaxChange](./getmaxchange/) | Le changement maximal pour résoudre une référence circulaire. |
| [SetMaxChange](./setmaxchange/) | Le changement maximal pour résoudre une référence circulaire. |
| [GetPrecisionAsDisplayed](./getprecisionasdisplayed/) | Indique si la précision du résultat calculé doit être définie telle qu'elle est affichée lors du calcul des formules. |
| [SetPrecisionAsDisplayed](./setprecisionasdisplayed/) | Indique si la précision du résultat calculé doit être définie telle qu'elle est affichée lors du calcul des formules. |
| [GetEnableCalculationChain](./getenablecalculationchain/) | Indique s'il faut activer la chaîne de calcul pour les formules. La valeur par défaut est false. |
| [SetEnableCalculationChain](./setenablecalculationchain/) | Indique s'il faut activer la chaîne de calcul pour les formules. La valeur par défaut est false. |
| [GetPreservePaddingSpaces](./getpreservepaddingspaces/) | Indique s'il faut préserver les espaces et les sauts de ligne qui sont insérés entre les jetons de formule lors de la récupération et de la définition des formules. La valeur par défaut est false. |
| [SetPreservePaddingSpaces](./setpreservepaddingspaces/) | Indique s'il faut préserver les espaces et les sauts de ligne qui sont insérés entre les jetons de formule lors de la récupération et de la définition des formules. La valeur par défaut est false. |

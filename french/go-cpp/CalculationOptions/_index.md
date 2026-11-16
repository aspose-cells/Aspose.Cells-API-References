---
title: "CalculationOptions Classe"
linktitle: "CalculationOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe CalculationOptions. Encapsule l'objet qui représente calculationoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/calculationoptions/
---

## CalculationOptions class

Représente les options de calcul.

```go

type CalculationOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewCalculationOptions](./newcalculationoptions/) | Constructeur par défaut. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetIgnoreError](./getignoreerror/) | Indique si les erreurs rencontrées lors du calcul des formules doivent être ignorées.L'erreur peut être une fonction non prise en charge, des liens externes, etc.La valeur par défaut est vraie. |
| [SetIgnoreError](./setignoreerror/) | Indique si les erreurs rencontrées lors du calcul des formules doivent être ignorées.L'erreur peut être une fonction non prise en charge, des liens externes, etc.La valeur par défaut est vraie. |
| [GetRecursive](./getrecursive/) | Indique s'il faut calculer les cellules dépendantes de manière récursive lors du calcul d'une cellule qui dépend d'autres cellules.La valeur par défaut est vraie. |
| [SetRecursive](./setrecursive/) | Indique s'il faut calculer les cellules dépendantes de manière récursive lors du calcul d'une cellule qui dépend d'autres cellules.La valeur par défaut est vraie. |
| [GetUserSpecifiedRefreshDynamicArrayFormula](./getuserspecifiedrefreshdynamicarrayformula/) | Indique si l'utilisateur a explicitement spécifié le comportement du rafraîchissement des formules de tableau dynamique avant de calculer les formules spécifiées. |
| [GetRefreshDynamicArrayFormula](./getrefreshdynamicarrayformula/) | Indique si les formules de tableau dynamique doivent être rafraîchies avant de calculer les formules. |
| [SetRefreshDynamicArrayFormula](./setrefreshdynamicarrayformula/) | Indique si les formules de tableau dynamique doivent être rafraîchies avant de calculer les formules. |
| [GetCustomEngine](./getcustomengine/) | Le moteur de calcul de formules personnalisé pour étendre le moteur de calcul par défaut d'Aspose.Cells. |
| [SetCustomEngine](./setcustomengine/) | Le moteur de calcul de formules personnalisé pour étendre le moteur de calcul par défaut d'Aspose.Cells. |
| [GetCalcStackSize](./getcalcstacksize/) | La taille de la pile pour le calcul récursif des cellules. La valeur par défaut est 200. |
| [SetCalcStackSize](./setcalcstacksize/) | La taille de la pile pour le calcul récursif des cellules. La valeur par défaut est 200. |
| [GetPrecisionStrategy](./getprecisionstrategy/) | Spécifie la stratégie de traitement de la précision du calcul. |
| [SetPrecisionStrategy](./setprecisionstrategy/) | Spécifie la stratégie de traitement de la précision du calcul. |
| [GetLinkedDataSources](./getlinkeddatasources/) | Spécifie les sources de données pour les liens externes utilisés dans les formules. |
| [SetLinkedDataSources](./setlinkeddatasources/) | Spécifie les sources de données pour les liens externes utilisés dans les formules. |
| [GetCharacterEncoding](./getcharacterencoding/) | Spécifie l'encodage utilisé pour l'encodage/décodage des caractères lors du calcul des formules. Pour des fonctions telles que CHAR, CODE, le résultat calculé dépend des paramètres régionaux et du jeu de caractères par défaut de l'environnement. Avec cette propriété, l'utilisateur peut spécifier l'encodage approprié utilisé pour ces fonctions afin d'obtenir le résultat attendu. |
| [SetCharacterEncoding](./setcharacterencoding/) | Spécifie l'encodage utilisé pour l'encodage/décodage des caractères lors du calcul des formules. Pour des fonctions telles que CHAR, CODE, le résultat calculé dépend des paramètres régionaux et du jeu de caractères par défaut de l'environnement. Avec cette propriété, l'utilisateur peut spécifier l'encodage approprié utilisé pour ces fonctions afin d'obtenir le résultat attendu. |

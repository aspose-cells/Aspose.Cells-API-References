---
title: "Classe AbstractCalculationEngine"
linktitle: "AbstractCalculationEngine"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe AbstractCalculationEngine. Encapsule l’objet qui représente abstractcalculationengine en Go."
type: docs
weight: 200
url: /fr/go-cpp/abstractcalculationengine/
---

## AbstractCalculationEngine class

Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells.

```go

type AbstractCalculationEngine struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |

## Méthodes

| Méthode | Description |
| --- | --- |
| [SkipCalculation](./skipcalculation/) | Ignore le calcul de toute la formule qui fait référence à la fonction actuellement évaluée. |
| [IsParamLiteralRequired](./isparamliteralrequired/) | Indique si ce moteur a besoin du texte littéral du paramètre lors d’un calcul. La valeur par défaut est false. |
| [IsParamArrayModeRequired](./isparamarraymoderequired/) | Indique si ce moteur a besoin que le paramètre soit calculé en mode tableau. La valeur par défaut est false. Si CalculationData.GetParamValueInArrayMode(int, int, int) est requis lors du calcul de customfunctions et que l’utilisateur n’a pas mis à jour la définition pour ceux‑ci (par Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)), cette propriété doit être définie sur true. |
| [GetProcessBuiltInFunctions](./getprocessbuiltinfunctions/) | Indique si les fonctions intégrées qui ont été prises en charge par le moteur intégré doivent être vérifiées et traitées par cette implémentation. La valeur par défaut est false. |
| [ForceRecalculate](./forcerecalculate/) | Indique s’il faut forcer la fonction donnée à être toujours recalculée lors du calcul des formules partagées. |

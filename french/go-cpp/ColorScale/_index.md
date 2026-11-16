---
title: "Classe ColorScale"
linktitle: "ColorScale"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe ColorScale. Encapsule l'objet qui représente colorscale en Go."
type: docs
weight: 200
url: /fr/go-cpp/colorscale/
---

## ColorScale class

Décrit la règle de mise en forme conditionnelle ColorScale. Cette règle de mise en forme conditionnelle crée une échelle de couleur graduée sur les cellules.

```go

type ColorScale struct  {
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
| [GetIs3ColorScale](./getis3colorscale/) | Indique si le formatage conditionnel est une échelle de couleur à 3 niveaux. |
| [SetIs3ColorScale](./setis3colorscale/) | Indique si le formatage conditionnel est une échelle de couleur à 3 niveaux. |
| [GetMinCfvo](./getmincfvo/) | Obtenir ou définir l'objet de valeur minimale de ce ColorScale. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Max. |
| [GetMidCfvo](./getmidcfvo/) | Obtenir ou définir l'objet de valeur médiane de ce ColorScale. Impossible de définir CFValueObject avec le type FormatConditionValueType.Max ou FormatConditionValueType.Min. |
| [GetMaxCfvo](./getmaxcfvo/) | Obtenir ou définir l'objet de valeur maximale de ce ColorScale. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Min. |
| [GetMinColor](./getmincolor/) | Obtenir ou définir la couleur du dégradé pour la valeur minimale dans la plage. |
| [SetMinColor](./setmincolor/) | Obtenir ou définir la couleur du dégradé pour la valeur minimale dans la plage. |
| [GetMidColor](./getmidcolor/) | Obtenir ou définir la couleur du dégradé pour la valeur médiane dans la plage. |
| [SetMidColor](./setmidcolor/) | Obtenir ou définir la couleur du dégradé pour la valeur médiane dans la plage. |
| [GetMaxColor](./getmaxcolor/) | Obtenir ou définir la couleur du dégradé pour la valeur maximale dans la plage. |
| [SetMaxColor](./setmaxcolor/) | Obtenir ou définir la couleur du dégradé pour la valeur maximale dans la plage. |

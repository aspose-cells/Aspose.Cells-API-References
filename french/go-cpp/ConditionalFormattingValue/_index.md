---
title: "Classe ConditionalFormattingValue"
linktitle: "ConditionalFormattingValue"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe ConditionalFormattingValue. Encapsule l'objet qui représente conditionalformattingvalue en Go."
type: docs
weight: 200
url: /fr/go-cpp/conditionalformattingvalue/
---

## ConditionalFormattingValue class

Décrit les valeurs des points d'interpolation dans une échelle graduée, une barre de données ou un jeu d'icônes.

```go

type ConditionalFormattingValue struct  {
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
| [GetValue](./getvalue/) | Obtient ou définit la valeur de cet objet de valeur de mise en forme conditionnelle. Il doit être utilisé en conjonction avec Type. |
| [SetValue](./setvalue/) | Obtient ou définit la valeur de cet objet de valeur de mise en forme conditionnelle. Il doit être utilisé en conjonction avec Type. |
| [GetType](./gettype/) | Obtient ou définit le type de cet objet de valeur de mise en forme conditionnelle. Définir le type sur FormatConditionValueType.Min ou FormatConditionValueType.Max définira automatiquement "Value" sur null. |
| [SetType](./settype/) | Obtient ou définit le type de cet objet de valeur de mise en forme conditionnelle. Définir le type sur FormatConditionValueType.Min ou FormatConditionValueType.Max définira automatiquement "Value" sur null. |
| [IsGTE](./isgte/) | Obtient ou définit le drapeau Supérieur ou égal. À n'utiliser que pour les jeux d'icônes, détermine si cette valeur seuil utilise l'opérateur supérieur ou égal. 'false' indique que 'supérieur' est utilisé au lieu de 'supérieur ou égal'. La valeur par défaut est true. |
| [SetIsGTE](./setisgte/) | Obtient ou définit le drapeau Supérieur ou égal. À n'utiliser que pour les jeux d'icônes, détermine si cette valeur seuil utilise l'opérateur supérieur ou égal. 'false' indique que 'supérieur' est utilisé au lieu de 'supérieur ou égal'. La valeur par défaut est true. |

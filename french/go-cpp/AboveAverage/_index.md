---
title: "Classe AboveAverage"
linktitle: "AboveAverage"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe AboveAverage. Encapsule l'objet qui représente aboveaverage en Go."
type: docs
weight: 200
url: /fr/go-cpp/aboveaverage/
---

## AboveAverage class

Décrivez la règle de mise en forme conditionnelle AboveAverage. Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui sont au-dessus ou en dessous de la moyenne pour toutes les valeurs de la plage.

```go

type AboveAverage struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewAboveAverage](./newaboveaverage/) | Constructeur par défaut. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [IsAboveAverage](./isaboveaverage/) | Obtenez ou définissez le drapeau indiquant si la règle est une règle « au‑dessus de la moyenne ». 'true' indique « au‑dessus de la moyenne ». Valeur par défaut est true. |
| [SetIsAboveAverage](./setisaboveaverage/) | Obtenez ou définissez le drapeau indiquant si la règle est une règle « au‑dessus de la moyenne ». 'true' indique « au‑dessus de la moyenne ». Valeur par défaut est true. |
| [IsEqualAverage](./isequalaverage/) | Obtenez ou définissez le drapeau indiquant si les critères 'aboveAverage' et 'belowAverage' sont inclusifs de la moyenne elle‑même, ou exclusifs de cette valeur. 'true' indique d'inclure la valeur moyenne dans les critères. Valeur par défaut est false. |
| [SetIsEqualAverage](./setisequalaverage/) | Obtenez ou définissez le drapeau indiquant si les critères 'aboveAverage' et 'belowAverage' sont inclusifs de la moyenne elle‑même, ou exclusifs de cette valeur. 'true' indique d'inclure la valeur moyenne dans les critères. Valeur par défaut est false. |
| [GetStdDev](./getstddev/) | Obtenez ou définissez le nombre d'écarts‑type à inclure au‑dessus ou au‑dessous de la moyenne dans la règle de mise en forme conditionnelle. La valeur d'entrée doit être comprise entre 0 et 3 (inclure 0 et 3). Définir cette valeur à 0 signifie que stdDev n'est pas défini. La valeur par défaut est 0. |
| [SetStdDev](./setstddev/) | Obtenez ou définissez le nombre d'écarts‑type à inclure au‑dessus ou au‑dessous de la moyenne dans la règle de mise en forme conditionnelle. La valeur d'entrée doit être comprise entre 0 et 3 (inclure 0 et 3). Définir cette valeur à 0 signifie que stdDev n'est pas défini. La valeur par défaut est 0. |

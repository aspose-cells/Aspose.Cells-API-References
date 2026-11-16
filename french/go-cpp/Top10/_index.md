---
title: "Classe Top10"
linktitle: "Top10"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe Top10. Encapsule l'objet qui représente top10 en Go."
type: docs
weight: 200
url: /fr/go-cpp/top10/
---

## Top10 class

Décrivez la règle de mise en forme conditionnelle Top10. Cette règle de mise en forme conditionnelle met en surbrillance les cellules dont les valeurs se situent dans la tranche supérieure ou inférieure N, selon spécification.

```go

type Top10 struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewTop10](./newtop10/) | Constructeur par défaut. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [IsPercent](./ispercent/) | Obtient ou définit si une règle "top/bottom n" est une règle "top/bottom n percent". Valeur par défaut : false. |
| [SetIsPercent](./setispercent/) | Obtient ou définit si une règle "top/bottom n" est une règle "top/bottom n percent". Valeur par défaut : false. |
| [IsBottom](./isbottom/) | Obtient ou définit si une règle "top/bottom n" est une règle "bottom n". Valeur par défaut : false. |
| [SetIsBottom](./setisbottom/) | Obtient ou définit si une règle "top/bottom n" est une règle "bottom n". Valeur par défaut : false. |
| [GetRank](./getrank/) | Obtient ou définit la valeur de "n" dans une règle de mise en forme conditionnelle "top/bottom n". Si IsPercent est vrai, la valeur doit être comprise entre 0 et 100. Sinon, elle doit être comprise entre 0 et 1000. Valeur par défaut : 10. |
| [SetRank](./setrank/) | Obtient ou définit la valeur de "n" dans une règle de mise en forme conditionnelle "top/bottom n". Si IsPercent est vrai, la valeur doit être comprise entre 0 et 100. Sinon, elle doit être comprise entre 0 et 1000. Valeur par défaut : 10. |

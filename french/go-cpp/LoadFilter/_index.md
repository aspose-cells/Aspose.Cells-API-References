---
title: "Classe LoadFilter"
linktitle: "LoadFilter"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe LoadFilter. Encapsule l'objet qui représente loadfilter en Go."
type: docs
weight: 200
url: /fr/go-cpp/loadfilter/
---

## LoadFilter class

Représente le filtre qui fournit des options de chargement des données lors du chargement du classeur à partir d'un modèle.

```go

type LoadFilter struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewLoadFilter](./newloadfilter/) | Construit un LoadFilter avec les options de filtre par défaut LoadDataFilterOptions::All. |
| [NewLoadFilter_LoadDataFilterOptions](./newloadfilter_loaddatafilteroptions/) | Construit un LoadFilter avec les options de filtre fournies. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetLoadDataFilterOptions](./getloaddatafilteroptions/) | Obtient les options de filtre pour indiquer quelles données doivent être chargées. |
| [SetLoadDataFilterOptions](./setloaddatafilteroptions/) | Définit les options de filtre pour indiquer quelles données doivent être chargées. |
| [GetSheetsInLoadingOrder](./getsheetsinloadingorder/) | Spécifie les feuilles (indices) et l'ordre à charger.Default est null, ce qui indique de charger toutes les feuilles dans l'ordre par défaut du fichier modèle.Si ce n'est pas null et que l'indice d'une feuille n'est pas dans le tableau retourné, alors la feuille ne sera pas chargée. |
| [StartSheet](./startsheet/) | Prépare les options de filtre avant de charger la feuille de calcul donnée.L'implémentation de LoadFilter par l'utilisateur peut modifier les LoadDataFilterOptions ici pour indiquer comment charger les données pour cette feuille de calcul. |

---
title: "Classe NameCollection"
linktitle: "NameCollection"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe NameCollection. Encapsule l'objet qui représente namecollection en Go."
type: docs
weight: 200
url: /fr/go-cpp/namecollection/
---

## NameCollection class

Représente une collection de tous les objets <see cref="Name"/> dans la feuille de calcul.

```go

type NameCollection struct  {
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
| [Add](./add/) | Définit un nouveau nom. |
| [Get_Int](./get_int/) | Obtient l'élément Name à l'index spécifié. |
| [Filter](./filter/) | Obtient tous les noms définis par portée. |
| [Get_String](./get_string/) | Obtient l'élément Name avec le nom spécifié. |
| [Remove_stringArray](./remove_stringarray/) | Supprime un tableau de noms |
| [Remove_String](./remove_string/) | Supprime le nom. |
| [RemoveAt](./removeat/) | Supprime le nom à l'index spécifique. |
| [Clear](./clear/) | Supprime tous les noms définis qui ne sont pas référencés par les formules et la source de données. Si le nom défini est référencé, nous ne faisons que définir Name.ReferTo à null et les masquer. |
| [RemoveDuplicateNames](./removeduplicatenames/) | Supprime les noms définis en double |
| [Sort](./sort/) | Trie les noms définis. |
| [GetCount](./getcount/) | Obtient le nombre d'éléments contenus dans l'instance. |

---
title: "Classe CustomDocumentPropertyCollection"
linktitle: "CustomDocumentPropertyCollection"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe CustomDocumentPropertyCollection. Encapsule l'objet qui représente customdocumentpropertycollection en Go."
type: docs
weight: 200
url: /fr/go-cpp/customdocumentpropertycollection/
---

## CustomDocumentPropertyCollection class

Une collection de propriétés de document personnalisées.

```go

type CustomDocumentPropertyCollection struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewCustomDocumentPropertyCollection](./newcustomdocumentpropertycollection/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [Add_String_String](./add_string_string/) | Crée une nouvelle propriété de document personnalisée du type de données <b>PropertyType.String</b>. |
| [Add_String_Int](./add_string_int/) | Crée une nouvelle propriété de document personnalisée du type de données <b>PropertyType.Number</b>. |
| [Add_String_Date](./add_string_date/) | Crée une nouvelle propriété de document personnalisée du type de données <b>PropertyType.DateTime</b>. |
| [Add_String_Bool](./add_string_bool/) | Crée une nouvelle propriété de document personnalisée du type de données <b>PropertyType.Boolean</b>. |
| [Add_String_Double](./add_string_double/) | Crée une nouvelle propriété de document personnalisée du type de données <b>PropertyType.Float</b>. |
| [AddLinkToContent](./addlinktocontent/) | Crée une nouvelle propriété de document personnalisée qui se lie au contenu. |
| [UpdateLinkedPropertyValue](./updatelinkedpropertyvalue/) | Met à jour les valeurs de toutes les propriétés personnalisées qui sont liées au contenu (utilise la valeur de la cellule de la plage liée pour mettre à jour la valeur de la propriété personnalisée). |
| [UpdateLinkedRange](./updatelinkedrange/) | Met à jour toutes les plages qui sont liées aux propriétés personnalisées (utilise la valeur de la propriété de document personnalisée pour mettre à jour la valeur de la cellule de la plage liée). |
| [Get_Int](./get_int/) | Renvoie un objet DocumentProperty par indice. |
| [Contains](./contains/) | Renvoie vrai si une propriété portant le nom spécifié existe dans la collection. |
| [IndexOf](./indexof/) | Obtient l'indice d'une propriété par son nom. |
| [Remove](./remove/) | Supprime une propriété portant le nom spécifié de la collection. |
| [RemoveAt](./removeat/) | Supprime une propriété à l'indice spécifié. |
| [GetCount](./getcount/) | Obtient le nombre d'éléments contenus dans l'instance. |

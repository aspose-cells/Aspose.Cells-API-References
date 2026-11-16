---
title: "ProtectedRange Classe"
linktitle: "ProtectedRange"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "ProtectedRange classe. Encapsule l'objet qui représente protectedrange en Go."
type: docs
weight: 200
url: /fr/go-cpp/protectedrange/
---

## ProtectedRange class

Une plage spécifiée autorisée à être modifiée lorsque la protection de la feuille est ACTIVÉE.

```go

type ProtectedRange struct  {
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
| [GetName](./getname/) | Obtient le titre de la plage. Ceci est utilisé comme un descripteur, pas comme une définition de plage nommée. |
| [SetName](./setname/) | Obtient le titre de la plage. Ceci est utilisé comme un descripteur, pas comme une définition de plage nommée. |
| [GetCellArea](./getcellarea/) | Obtient l'objet CellArea qui représente la zone de cellules à protéger. |
| [GetAreas](./getareas/) | Obtient toutes les zones référencées. |
| [AddArea](./addarea/) | Ajoute une zone référencée à cet objet. |
| [IsProtectedWithPassword](./isprotectedwithpassword/) | Indique si les feuilles de calcul sont protégées par un mot de passe. |
| [GetPassword](./getpassword/) | Représente le mot de passe pour protéger la plage. |
| [SetPassword](./setpassword/) | Représente le mot de passe pour protéger la plage. |
| [GetSecurityDescriptor](./getsecuritydescriptor/) | Le descripteur de sécurité définit les comptes d'utilisateur qui peuvent modifier cette plage sans fournir de mot de passe pour y accéder. |
| [SetSecurityDescriptor](./setsecuritydescriptor/) | Le descripteur de sécurité définit les comptes d'utilisateur qui peuvent modifier cette plage sans fournir de mot de passe pour y accéder. |

---
title: "Classe AbstractLowCodeSaveOptionsProvider"
linktitle: "AbstractLowCodeSaveOptionsProvider"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe AbstractLowCodeSaveOptionsProvider. Encapsule l'objet qui représente abstractlowcodesaveoptionsprovider en Go."
type: docs
weight: 200
url: /fr/go-cpp/abstractlowcodesaveoptionsprovider/
---

## AbstractLowCodeSaveOptionsProvider class

Implémentation pour fournir plusieurs options d'enregistrement pour les processus qui nécessitent plusieurs sorties. Par exemple, la fonctionnalité <see cref=\"SpreadsheetSplitter\"/> nécessite plusieurs destinations pour enregistrer les fichiers découpés.

```go

type AbstractLowCodeSaveOptionsProvider struct  {
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
| [GetSaveOptions](./getsaveoptions/) | Obtient les options d'enregistrement à partir desquelles récupérer les paramètres de sortie pour la partie actuellement divisée. Retourner null indique d'ignorer la partie donnée. |
| [Finish](./finish/) | Libère les ressources après le traitement de la partie actuellement divisée. |

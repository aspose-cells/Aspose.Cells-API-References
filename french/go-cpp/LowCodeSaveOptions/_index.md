---
title: "Classe LowCodeSaveOptions"
linktitle: "LowCodeSaveOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe LowCodeSaveOptions. Encapsule l'objet qui représente lowcodesaveoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/lowcodesaveoptions/
---

## LowCodeSaveOptions class

Options pour enregistrer les résultats générés de manière low code.

```go

type LowCodeSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewLowCodeSaveOptions](./newlowcodesaveoptions/) | Constructeur par défaut. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetOutputFile](./getoutputfile/) | Obtient et définit le fichier(avec le chemin si nécessaire) pour enregistrer les données générées. Lors de la définition de cette propriété avec une valeur différente de null ou d'une chaîne vide, OutputStream sera ignoré. |
| [SetOutputFile](./setoutputfile/) | Obtient et définit le fichier(avec le chemin si nécessaire) pour enregistrer les données générées. Lors de la définition de cette propriété avec une valeur différente de null ou d'une chaîne vide, OutputStream sera ignoré. |
| [GetOutputStream](./getoutputstream/) | Obtient et définit le flux pour écrire les données générées. Lors de la définition de cette propriété avec une valeur différente de null, OutputFile sera ignoré. |
| [SetOutputStream](./setoutputstream/) | Obtient et définit le flux pour écrire les données générées. Lors de la définition de cette propriété avec une valeur différente de null, OutputFile sera ignoré. |
| [GetSaveFormat](./getsaveformat/) | Obtient et définit le format d'enregistrement pour la sortie. En général, pour un processus spécifique en low code, seuls certains formats spécifiques sont autorisés. Veuillez spécifier le format correct pour le processus correspondant, sinon un résultat inattendu ou même une exception peut survenir. |
| [SetSaveFormat](./setsaveformat/) | Obtient et définit le format d'enregistrement pour la sortie. En général, pour un processus spécifique en low code, seuls certains formats spécifiques sont autorisés. Veuillez spécifier le format correct pour le processus correspondant, sinon un résultat inattendu ou même une exception peut survenir. |

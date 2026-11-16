---
title: "Classe LowCodePdfSaveOptions"
linktitle: "LowCodePdfSaveOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe LowCodePdfSaveOptions. Encapsule l'objet qui représente lowcodepdfsaveoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/lowcodepdfsaveoptions/
---

## LowCodePdfSaveOptions class

Options pour enregistrer le pdf de manière low code.

```go

type LowCodePdfSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewLowCodePdfSaveOptions](./newlowcodepdfsaveoptions/) | Constructeur par défaut. |
| [NewLowCodePdfSaveOptions_LowCodeSaveOptions](./newlowcodepdfsaveoptions_lowcodesaveoptions/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetSaveFormat](./getsaveformat/) | Le format d'enregistrement pour la sortie. Pour la conversion en pdf, il ne peut être que SaveFormat.Pdf. |
| [SetSaveFormat](./setsaveformat/) | Le format d'enregistrement pour la sortie. Pour la conversion en pdf, il ne peut être que SaveFormat.Pdf. |
| [GetPdfOptions](./getpdfoptions/) | Les options pour enregistrer le fichier Pdf. |
| [SetPdfOptions](./setpdfoptions/) | Les options pour enregistrer le fichier Pdf. |
| [GetOutputFile](./getoutputfile/) | Obtient et définit le fichier(avec le chemin si nécessaire) pour enregistrer les données générées. Lors de la définition de cette propriété avec une valeur différente de null ou d'une chaîne vide, OutputStream sera ignoré. |
| [SetOutputFile](./setoutputfile/) | Obtient et définit le fichier(avec le chemin si nécessaire) pour enregistrer les données générées. Lors de la définition de cette propriété avec une valeur différente de null ou d'une chaîne vide, OutputStream sera ignoré. |
| [GetOutputStream](./getoutputstream/) | Obtient et définit le flux pour écrire les données générées. Lors de la définition de cette propriété avec une valeur différente de null, OutputFile sera ignoré. |
| [SetOutputStream](./setoutputstream/) | Obtient et définit le flux pour écrire les données générées. Lors de la définition de cette propriété avec une valeur différente de null, OutputFile sera ignoré. |

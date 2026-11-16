---
title: "Classe LowCodeSaveOptionsProviderOfPlaceHolders"
linktitle: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe LowCodeSaveOptionsProviderOfPlaceHolders. Encapsule l'objet qui représente lowcodesaveoptionsproviderofplaceholders en Go."
type: docs
weight: 200
url: /fr/go-cpp/lowcodesaveoptionsproviderofplaceholders/
---

## LowCodeSaveOptionsProviderOfPlaceHolders class

Implémentation pour fournir des options d'enregistrement qui sauvegardent les parties découpées dans des fichiers et le chemin du fichier résultant est défini avec des espaces réservés.

```go

type LowCodeSaveOptionsProviderOfPlaceHolders struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_String](./newlowcodesaveoptionsproviderofplaceholders_string/) | Instancie une instance pour fournir des options d'enregistrement selon les modèles spécifiés. |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofplaceholders_abstractlowcodesaveoptionsprovider/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetSheetIndexOffset](./getsheetindexoffset/) | Décalage de l'index de la feuille entre celui utilisé dans le chemin de fichier et sa valeur réelle (SplitPartInfo.SheetIndex). |
| [SetSheetIndexOffset](./setsheetindexoffset/) | Décalage de l'index de la feuille entre celui utilisé dans le chemin de fichier et sa valeur réelle (SplitPartInfo.SheetIndex). |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | Décalage de l'index de la partie découpée entre celui utilisé dans le chemin de fichier et sa valeur réelle (SplitPartInfo.PartIndex). |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | Décalage de l'index de la partie découpée entre celui utilisé dans le chemin de fichier et sa valeur réelle (SplitPartInfo.PartIndex). |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | Indique s'il faut toujours ajouter l'index ou le nom de la feuille au chemin du fichier. La valeur par défaut est false, c'est‑dira que lorsqu'il n'y a qu'une seule feuille, l'index et le nom de la feuille ainsi que le préfixe correspondant (SheetNamePrefix) ne seront pas ajoutés au chemin du fichier. |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | Indique s'il faut toujours ajouter l'index ou le nom de la feuille au chemin du fichier. La valeur par défaut est false, c'est‑dira que lorsqu'il n'y a qu'une seule feuille, l'index et le nom de la feuille ainsi que le préfixe correspondant (SheetNamePrefix) ne seront pas ajoutés au chemin du fichier. |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | Indique s'il faut toujours ajouter l'index de la partie découpée au chemin du fichier. La valeur par défaut est false, c'est‑dira que lorsqu'il n'y a qu'une seule partie découpée, l'index de la partie découpée ainsi que le préfixe correspondant (SplitPartPrefix) ne seront pas ajoutés au chemin du fichier. |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | Indique s'il faut toujours ajouter l'index de la partie découpée au chemin du fichier. La valeur par défaut est false, c'est‑dira que lorsqu'il n'y a qu'une seule partie découpée, l'index de la partie découpée ainsi que le préfixe correspondant (SplitPartPrefix) ne seront pas ajoutés au chemin du fichier. |
| [GetSheetNamePrefix](./getsheetnameprefix/) | Préfixe pour l'index de la feuille de calcul. |
| [SetSheetNamePrefix](./setsheetnameprefix/) | Préfixe pour l'index de la feuille de calcul. |
| [GetSheetIndexPrefix](./getsheetindexprefix/) | Préfixe pour l'index de la feuille de calcul. |
| [SetSheetIndexPrefix](./setsheetindexprefix/) | Préfixe pour l'index de la feuille de calcul. |
| [GetSplitPartPrefix](./getsplitpartprefix/) | Préfixe pour l'index de la partie découpée. |
| [SetSplitPartPrefix](./setsplitpartprefix/) | Préfixe pour l'index de la partie découpée. |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | Le modèle pour créer une instance d'options d'enregistrement dans GetSaveOptions(SplitPartInfo). |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | Le modèle pour créer une instance d'options d'enregistrement dans GetSaveOptions(SplitPartInfo). |
| [GetSaveOptions](./getsaveoptions/) | Obtient les options d'enregistrement à partir desquelles récupérer les paramètres de sortie pour la partie découpée actuelle. |
| [Finish](./finish/) | Libère les ressources après le traitement de la partie actuellement divisée. |

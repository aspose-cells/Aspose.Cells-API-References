---
title: "LowCodeSaveOptionsProviderOfAssembling Classe"
linktitle: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "LowCodeSaveOptionsProviderOfAssembling classe. Encapsule l'objet qui représente lowcodesaveoptionsproviderofassembling en Go."
type: docs
weight: 200
url: /fr/go-cpp/lowcodesaveoptionsproviderofassembling/
---

## LowCodeSaveOptionsProviderOfAssembling class

Implémentation pour fournir des options d'enregistrement qui sauvegardent les parties découpées dans des fichiers et le chemin du fichier résultant est nommé comme (il peut contenir des répertoires) :<see cref=\"PathHeader\"/>+<see cref=\"SheetPrefix\"/>+SheetIndex(ou SheetName)+<see cref=\"SplitPartPrefix\"/>+SplitPartIndex+<see cref=\"PathTail\"/>.

```go

type LowCodeSaveOptionsProviderOfAssembling struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfAssembling](./newlowcodesaveoptionsproviderofassembling/) | Constructeur par défaut. |
| [NewLowCodeSaveOptionsProviderOfAssembling_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofassembling_abstractlowcodesaveoptionsprovider/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetPathHeader](./getpathheader/) | Partie d'en-tête (avant le contenu ajouté de la feuille et de la partie découpée) du chemin de fichier. |
| [SetPathHeader](./setpathheader/) | Partie d'en-tête (avant le contenu ajouté de la feuille et de la partie découpée) du chemin de fichier. |
| [GetPathTail](./getpathtail/) | Partie finale (après les numéros de séquence) du chemin de fichier. Elle doit inclure l'extension du nom de fichier. |
| [SetPathTail](./setpathtail/) | Partie finale (après les numéros de séquence) du chemin de fichier. Elle doit inclure l'extension du nom de fichier. |
| [GetUseSheetName](./getusesheetname/) | Indique si le chemin de fichier est construit avec le nom de la feuille au lieu de l'index de la feuille. La valeur par défaut est false. |
| [SetUseSheetName](./setusesheetname/) | Indique si le chemin de fichier est construit avec le nom de la feuille au lieu de l'index de la feuille. La valeur par défaut est false. |
| [GetSheetPrefix](./getsheetprefix/) | Préfixe pour l'index de la feuille de calcul. |
| [SetSheetPrefix](./setsheetprefix/) | Préfixe pour l'index de la feuille de calcul. |
| [GetSplitPartPrefix](./getsplitpartprefix/) | Préfixe pour l'index de la partie découpée. |
| [SetSplitPartPrefix](./setsplitpartprefix/) | Préfixe pour l'index de la partie découpée. |
| [GetSheetIndexOffset](./getsheetindexoffset/) | Décalage de l'index de la feuille entre celui utilisé dans le chemin de fichier et sa valeur réelle (SplitPartInfo.SheetIndex). |
| [SetSheetIndexOffset](./setsheetindexoffset/) | Décalage de l'index de la feuille entre celui utilisé dans le chemin de fichier et sa valeur réelle (SplitPartInfo.SheetIndex). |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | Décalage de l'index de la partie découpée entre celui utilisé dans le chemin de fichier et sa valeur réelle (SplitPartInfo.PartIndex). |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | Décalage de l'index de la partie découpée entre celui utilisé dans le chemin de fichier et sa valeur réelle (SplitPartInfo.PartIndex). |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | Indique si l'index ou le nom de la feuille doit toujours être ajouté au chemin de fichier. La valeur par défaut est false, c'est‑à‑dire que lorsqu'il n'y a qu'une seule feuille, l'index (ou le nom) de la feuille et le préfixe correspondant ne seront pas ajoutés au chemin de fichier. |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | Indique si l'index ou le nom de la feuille doit toujours être ajouté au chemin de fichier. La valeur par défaut est false, c'est‑à‑dire que lorsqu'il n'y a qu'une seule feuille, l'index (ou le nom) de la feuille et le préfixe correspondant ne seront pas ajoutés au chemin de fichier. |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | Indique si l'index de la partie découpée doit toujours être ajouté au chemin de fichier. La valeur par défaut est false, c'est‑à‑dire que lorsqu'il n'y a qu'une seule partie découpée, l'index de la partie découpée et le préfixe correspondant ne seront pas ajoutés au chemin de fichier. |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | Indique si l'index de la partie découpée doit toujours être ajouté au chemin de fichier. La valeur par défaut est false, c'est‑à‑dire que lorsqu'il n'y a qu'une seule partie découpée, l'index de la partie découpée et le préfixe correspondant ne seront pas ajoutés au chemin de fichier. |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | Le modèle pour créer une instance d'options d'enregistrement dans GetSaveOptions(SplitPartInfo). |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | Le modèle pour créer une instance d'options d'enregistrement dans GetSaveOptions(SplitPartInfo). |
| [GetSaveOptions](./getsaveoptions/) | Obtient les options d'enregistrement à partir desquelles récupérer les paramètres de sortie pour la partie découpée actuelle. |
| [Finish](./finish/) | Libère les ressources après le traitement de la partie actuellement divisée. |

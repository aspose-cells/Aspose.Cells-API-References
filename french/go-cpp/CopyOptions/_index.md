---
title: "CopyOptions Classe"
linktitle: "CopyOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe CopyOptions. Encapsule l'objet qui représente copyoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/copyoptions/
---

## CopyOptions class

Représente les options de copie.

```go

type CopyOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewCopyOptions](./newcopyoptions/) | Constructeur CopyOptions. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetKeepMacros](./getkeepmacros/) | Indique si les macros sont conservées ; |
| [SetKeepMacros](./setkeepmacros/) | Indique si les macros sont conservées ; |
| [GetExtendToAdjacentRange](./getextendtoadjacentrange/) | Indique s'il faut étendre les plages lors de la copie de la plage vers la plage adjacente. |
| [SetExtendToAdjacentRange](./setextendtoadjacentrange/) | Indique s'il faut étendre les plages lors de la copie de la plage vers la plage adjacente. |
| [GetCopyNames](./getcopynames/) | Indique s'il faut copier les noms. |
| [SetCopyNames](./setcopynames/) | Indique s'il faut copier les noms. |
| [GetCopyInvalidFormulasAsValues](./getcopyinvalidformulasasvalues/) | Si la formule n'est pas valide pour la destination cible, copier uniquement les valeurs. |
| [SetCopyInvalidFormulasAsValues](./setcopyinvalidformulasasvalues/) | Si la formule n'est pas valide pour la destination cible, copier uniquement les valeurs. |
| [GetColumnCharacterWidth](./getcolumncharacterwidth/) | Indique s'il faut copier la largeur des colonnes en unités de caractères. |
| [SetColumnCharacterWidth](./setcolumncharacterwidth/) | Indique s'il faut copier la largeur des colonnes en unités de caractères. |
| [GetReferToSheetWithSameName](./getrefertosheetwithsamename/) | Dans MS Excel, lors de la copie de formules qui font référence à d'autres feuilles de calcul pendant la copie d'une feuille vers une autre, les formules copiées doivent faire référence au classeur source. Cependant, dans certaines situations l'utilisateur peut avoir besoin que les formules copiées fassent référence à des feuilles de calcul portant le même nom dans le même classeur, par exemple lorsque ces feuilles ont déjà été copiées avant cette opération de copie, alors cette propriété doit être définie sur vrai. |
| [SetReferToSheetWithSameName](./setrefertosheetwithsamename/) | Dans MS Excel, lors de la copie de formules qui font référence à d'autres feuilles de calcul pendant la copie d'une feuille vers une autre, les formules copiées doivent faire référence au classeur source. Cependant, dans certaines situations l'utilisateur peut avoir besoin que les formules copiées fassent référence à des feuilles de calcul portant le même nom dans le même classeur, par exemple lorsque ces feuilles ont déjà été copiées avant cette opération de copie, alors cette propriété doit être définie sur vrai. |
| [GetReferToDestinationSheet](./getrefertodestinationsheet/) | Lors de la copie de la plage dans le même fichier et que le graphique fait référence à la feuille source, False signifie que la source de données du graphique copié ne sera pas modifiée. True signifie que la source de données du graphique copié fait référence à la feuille de destination. |
| [SetReferToDestinationSheet](./setrefertodestinationsheet/) | Lors de la copie de la plage dans le même fichier et que le graphique fait référence à la feuille source, False signifie que la source de données du graphique copié ne sera pas modifiée. True signifie que la source de données du graphique copié fait référence à la feuille de destination. |
| [GetUpdateInvalidReferencesToTargetSheet](./getupdateinvalidreferencestotargetsheet/) | Indique s'il faut se référer à la feuille de calcul cible si la feuille référencée n'est pas copiée. |
| [SetUpdateInvalidReferencesToTargetSheet](./setupdateinvalidreferencestotargetsheet/) | Indique s'il faut se référer à la feuille de calcul cible si la feuille référencée n'est pas copiée. |

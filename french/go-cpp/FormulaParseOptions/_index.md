---
title: "Classe FormulaParseOptions"
linktitle: "FormulaParseOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe FormulaParseOptions. Encapsule l'objet qui représente formulaparseoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/formulaparseoptions/
---

## FormulaParseOptions class

Représente les options lors de l'analyse d'une formule.

```go

type FormulaParseOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewFormulaParseOptions](./newformulaparseoptions/) | Constructeur par défaut. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetLocaleDependent](./getlocaledependent/) | Indique si la formule est formatée selon la locale. La valeur par défaut est false. |
| [SetLocaleDependent](./setlocaledependent/) | Indique si la formule est formatée selon la locale. La valeur par défaut est false. |
| [GetR1C1Style](./getr1c1style/) | Indique si la formule utilise le style de référence R1C1. La valeur par défaut est false. |
| [SetR1C1Style](./setr1c1style/) | Indique si la formule utilise le style de référence R1C1. La valeur par défaut est false. |
| [GetCheckAddIn](./getcheckaddin/) | Indique s'il faut vérifier les compléments dans les liens externes existants du classeur actuel pour les fonctions définies par l'utilisateur sans lien externe. La valeur par défaut est true(si la fonction définie par l'utilisateur correspond à un complément présent dans les liens externes existants, alors il est considéré comme le complément). |
| [SetCheckAddIn](./setcheckaddin/) | Indique s'il faut vérifier les compléments dans les liens externes existants du classeur actuel pour les fonctions définies par l'utilisateur sans lien externe. La valeur par défaut est true(si la fonction définie par l'utilisateur correspond à un complément présent dans les liens externes existants, alors il est considéré comme le complément). |
| [GetParse](./getparse/) | Indique s'il faut analyser la formule donnée. La valeur par défaut est true. Si elle est false, la chaîne de formule fournie sera conservée telle quelle pour la cellule jusqu'à ce que l'utilisateur appelle d'autres méthodes pour les analyser ou que les données de formule analysée soient requises par d'autres opérations telles que le calcul des formules. |
| [SetParse](./setparse/) | Indique s'il faut analyser la formule donnée. La valeur par défaut est true. Si elle est false, la chaîne de formule fournie sera conservée telle quelle pour la cellule jusqu'à ce que l'utilisateur appelle d'autres méthodes pour les analyser ou que les données de formule analysée soient requises par d'autres opérations telles que le calcul des formules. |
| [GetCustomFunctionDefinition](./getcustomfunctiondefinition/) | Définition de l'analyse des fonctions personnalisées. |
| [SetCustomFunctionDefinition](./setcustomfunctiondefinition/) | Définition de l'analyse des fonctions personnalisées. |

---
title: "Enumération EquationNodeType"
linktitle: "EquationNodeType"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Enumération EquationNodeType. Encapsule l'objet qui représente equationnodetype en Go."
type: docs
weight: 200
url: /fr/go-cpp/equationnodetype/
---

## EquationNodeType Enum

Type de nœud d'équation. Remarque :(1)[1-99] Actuellement il n'y a qu'un seul nœud dans la portée, et sa valeur d'énumération est 1. Le nœud qu'il spécifie est utilisé pour stocker du texte mathématique.(2)[100-199] Indique que le nœud est un composant de certains nœuds de fonctions spéciales.(3)[200-] Indique que le nœud possède des fonctions spéciales.

```go

type EquationNodeType int32


```

## Champs

| Champ | Description |
| --- | --- |
| [UnKnow](./unknow/) | Inconnu |
| [Text](./text/) | spécifie un nœud qui stocke du texte mathématique |
| [Base](./base/) | Spécifie un composant de base |
| [Denominator](./denominator/) | Spécifie un composant de dénominateur |
| [Numerator](./numerator/) | Spécifie un composant de numérateur |
| [FunctionName](./functionname/) | Spécifie un composant FunctionName |
| [Subscript](./subscript/) | Spécifie un composant de sous-script |
| [Superscript](./superscript/) | Spécifie un composant Superscript |
| [Degree](./degree/) | Spécifie un composant de degré |
| [MatrixRow](./matrixrow/) | Spécifie un composant MatrixRow.Une seule ligne de la matrice |
| [Limit](./limit/) | Représente un sous-objet de la fonction Lower-Limit ou de la fonction Upper-Limit |
| [EquationParagraph](./equationparagraph/) | Spécifie un paragraphe mathématique(oMathPara). |
| [LowerLimit](./lowerlimit/) | Spécifie la fonction Lower-Limit |
| [UpperLimit](./upperlimit/) | Spécifie la fonction Upper-Limit |
| [Mathematical](./mathematical/) | Spécifie une équation ou une expression mathématique(OMath). |
| [Fraction](./fraction/) | Spécifie une équation fractionnaire |
| [Function](./function/) | Spécifie une équation de fonction |
| [Delimiter](./delimiter/) | Spécifie une équation delimiter |
| [Nary](./nary/) | Spécifie une équation d'opérateur n-aire |
| [Radical](./radical/) | Spécifie l'équation radicale |
| [Sup](./sup/) | Spécifie une équation superscript |
| [Sub](./sub/) | Spécifie l'équation en indice |
| [SubSup](./subsup/) | Spécifie une équation avec des exposants et des indices à droite des opérandes. |
| [PreSubSup](./presubsup/) | Spécifie une équation avec des exposants et des indices à gauche des opérandes. |
| [Accent](./accent/) | Spécifie une équation d'accent |
| [Bar](./bar/) | Spécifie une équation à barre |
| [BorderBox](./borderbox/) | Spécifie une équation de boîte à bordure |
| [Box](./box/) | Spécifie une équation de boîte |
| [GroupChr](./groupchr/) | Spécifie une équation de groupe-caractère |
| [Matrix](./matrix/) | Spécifie l'équation de matrice, |
| [ArrayEquation](./arrayequation/) | Spécifie la fonction Equation-Array. La fonction consiste en une ou plusieurs équations. |

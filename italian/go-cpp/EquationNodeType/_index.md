---
title: "Enum EquationNodeType"
linktitle: "EquationNodeType"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Enum EquationNodeType. Incapsula l'oggetto che rappresenta equationnodetype in Go."
type: docs
weight: 200
url: /it/go-cpp/equationnodetype/
---

## EquationNodeType Enum

Tipo di nodo di equazione. Nota:(1)[1-99] Attualmente c'è solo un nodo nell'ambito, e il suo valore di enumerazione è 1. Il nodo specificato è usato per memorizzare testo matematico.(2)[100-199] Indica che il nodo è un componente di alcuni nodi di funzioni speciali.(3)[200-] Indica che il nodo ha alcune funzioni speciali.

```go

type EquationNodeType int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [UnKnow](./unknow/) | Sconosciuto |
| [Text](./text/) | specifica un nodo che memorizza testo matematico |
| [Base](./base/) | Specifica un componente Base |
| [Denominator](./denominator/) | Specifica un componente Denominatore |
| [Numerator](./numerator/) | Specifica un componente Numeratore |
| [FunctionName](./functionname/) | Specifica un componente FunctionName |
| [Subscript](./subscript/) | Specifica un componente Subscript |
| [Superscript](./superscript/) | Specifica un componente Superscript |
| [Degree](./degree/) | Specifica un componente Degree |
| [MatrixRow](./matrixrow/) | Specifica un componente MatrixRow. Una singola riga della matrice |
| [Limit](./limit/) | Rappresenta un sotto-oggetto della funzione Lower-Limit o Upper-Limit |
| [EquationParagraph](./equationparagraph/) | Specifica un paragrafo matematico (oMathPara). |
| [LowerLimit](./lowerlimit/) | Specifica la funzione Lower-Limit |
| [UpperLimit](./upperlimit/) | Specifica la funzione Upper-Limit |
| [Mathematical](./mathematical/) | Specifica un'equazione o un'espressione matematica (OMath). |
| [Fraction](./fraction/) | Specifica un'equazione frazionaria |
| [Function](./function/) | Specifica un'equazione di funzione |
| [Delimiter](./delimiter/) | Specifica un'equazione delimitatore |
| [Nary](./nary/) | Specifica un'equazione di operatore n-ario |
| [Radical](./radical/) | Specifica l'equazione radicale |
| [Sup](./sup/) | Specifica l'equazione superscript |
| [Sub](./sub/) | Specifica l'equazione con pedice |
| [SubSup](./subsup/) | Specifica un'equazione con apici e pedici a destra degli operandi. |
| [PreSubSup](./presubsup/) | Specifica un'equazione con apici e pedici a sinistra degli operandi. |
| [Accent](./accent/) | Specifica l'equazione di accento |
| [Bar](./bar/) | Specifica l'equazione a barra |
| [BorderBox](./borderbox/) | Specifica l'equazione del riquadro bordato |
| [Box](./box/) | Specifica l'equazione del riquadro |
| [GroupChr](./groupchr/) | Specifica l'equazione Gruppo-Carattere |
| [Matrix](./matrix/) | Specifica l'equazione Matrice, |
| [ArrayEquation](./arrayequation/) | Specifica la funzione Equation-Array. La funzione consiste in una o più equazioni. |

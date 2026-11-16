---
title: "EquationNodeType Enum"
linktitle: "EquationNodeType"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "EquationNodeType enum. Kapselt das Objekt, das equationnodetype in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/equationnodetype/
---

## EquationNodeType Enum

Gleichungsknoten-Typ. Hinweis:(1)[1-99] Derzeit gibt es nur einen Knoten im Geltungsbereich, und sein Enumerationswert ist 1. Der angegebene Knoten wird verwendet, um mathematischen Text zu speichern. (2)[100-199] Gibt an, dass der Knoten ein Bestandteil einiger spezieller Funktionsknoten ist. (3)[200-] Gibt an, dass der Knoten einige Sonderfunktionen hat.

```go

type EquationNodeType int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [UnKnow](./unknow/) | UnKnow |
| [Text](./text/) | gibt einen Knoten an, der mathematischen Text speichert |
| [Base](./base/) | Gibt eine Basis-Komponente an |
| [Denominator](./denominator/) | Gibt eine Nenner-Komponente an |
| [Numerator](./numerator/) | Gibt eine Zähler-Komponente an |
| [FunctionName](./functionname/) | Gibt eine FunctionName-Komponente an |
| [Subscript](./subscript/) | Gibt eine Subscript-Komponente an |
| [Superscript](./superscript/) | Gibt eine Superscript-Komponente an |
| [Degree](./degree/) | Gibt eine Degree-Komponente an |
| [MatrixRow](./matrixrow/) | Gibt eine MatrixRow-Komponente an. Eine einzelne Zeile der Matrix |
| [Limit](./limit/) | Stellt ein Subobjekt der Lower-Limit-Funktion oder Upper-Limit-Funktion dar |
| [EquationParagraph](./equationparagraph/) | Gibt einen mathematischen Absatz(oMathPara) an. |
| [LowerLimit](./lowerlimit/) | Gibt die Lower-Limit-Funktion an |
| [UpperLimit](./upperlimit/) | Gibt die Upper-Limit-Funktion an |
| [Mathematical](./mathematical/) | Gibt eine Gleichung oder mathematischen Ausdruck(OMath) an. |
| [Fraction](./fraction/) | Gibt eine Bruchgleichung an |
| [Function](./function/) | Gibt eine Funktionsgleichung an |
| [Delimiter](./delimiter/) | Gibt eine Trennzeichen-Gleichung an |
| [Nary](./nary/) | Gibt eine n-äre Operator-Gleichung an |
| [Radical](./radical/) | Gibt die Radikalgleichung an |
| [Sup](./sup/) | Gibt die Superscript-Gleichung an |
| [Sub](./sub/) | Gibt die Subscript-Gleichung an |
| [SubSup](./subsup/) | Gibt eine Gleichung mit Superscripts und Subscripts rechts von den Operanden an. |
| [PreSubSup](./presubsup/) | Gibt eine Gleichung mit Superscripts und Subscripts links von den Operanden an. |
| [Accent](./accent/) | Gibt eine Akzentgleichung an |
| [Bar](./bar/) | Gibt eine Balkengleichung an |
| [BorderBox](./borderbox/) | Gibt eine Rahmen-Box-Gleichung an |
| [Box](./box/) | Gibt eine Box-Gleichung an |
| [GroupChr](./groupchr/) | Gibt eine Group-Character-Gleichung an |
| [Matrix](./matrix/) | Gibt die Matrix-Gleichung an, |
| [ArrayEquation](./arrayequation/) | Gibt die Equation-Array-Funktion an. Die Funktion besteht aus einer oder mehreren Gleichungen. |

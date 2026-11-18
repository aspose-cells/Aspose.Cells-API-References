---
title: "EquationNodeType Enum"
linktitle: "EquationNodeType"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "EquationNodeType enum. Inkapslar objektet som representerar equationnodetype i Go."
type: docs
weight: 200
url: /sv/go-cpp/equationnodetype/
---

## EquationNodeType Enum

Ekvationsnodtyp. Obs:(1)[1-99] För närvarande finns det bara en nod i området, och dess uppräkningsvärde är 1. Noden den anger används för att lagra matematisk text.(2)[100-199] Indikerar att noden är en komponent av vissa specialfunktionsnoder.(3)[200-] Indikerar att noden har vissa specialfunktioner.

```go

type EquationNodeType int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [UnKnow](./unknow/) | Okänd |
| [Text](./text/) | specificerar en nod som lagrar matematisk text |
| [Base](./base/) | Specificerar en Base-komponent |
| [Denominator](./denominator/) | Specificerar en Denominator-komponent |
| [Numerator](./numerator/) | Specificerar en Numerator-komponent |
| [FunctionName](./functionname/) | Specificerar en FunctionName-komponent |
| [Subscript](./subscript/) | Specificerar en Subscript-komponent |
| [Superscript](./superscript/) | Specificerar en Superscript-komponent |
| [Degree](./degree/) | Specificerar en Degree-komponent |
| [MatrixRow](./matrixrow/) | Specificerar en MatrixRow-komponent. En enda rad i matrisen |
| [Limit](./limit/) | Representerar ett delobjekt av Lower-Limit-funktionen eller Upper-Limit-funktionen |
| [EquationParagraph](./equationparagraph/) | Anger ett matematiskt stycke(oMathPara). |
| [LowerLimit](./lowerlimit/) | Anger funktionen Lower-Limit. |
| [UpperLimit](./upperlimit/) | Anger funktionen Upper-Limit. |
| [Mathematical](./mathematical/) | Anger en ekvation eller matematiskt uttryck(OMath). |
| [Fraction](./fraction/) | Anger bråkequation. |
| [Function](./function/) | Anger funktionsekvation. |
| [Delimiter](./delimiter/) | Anger avgränsareekvation. |
| [Nary](./nary/) | Anger n-är operator-ekvation. |
| [Radical](./radical/) | Anger radikalekvation. |
| [Sup](./sup/) | Anger upphöjd ekvation. |
| [Sub](./sub/) | Anger nedsänkt ekvation. |
| [SubSup](./subsup/) | Anger en ekvation med upphöjda och nedsänkta tecken till höger om operanderna. |
| [PreSubSup](./presubsup/) | Anger en ekvation med upphöjda och nedsänkta tecken till vänster om operanderna. |
| [Accent](./accent/) | Anger accentekvation. |
| [Bar](./bar/) | Anger stapel-ekvation. |
| [BorderBox](./borderbox/) | Anger kantboxekvation. |
| [Box](./box/) | Anger boxekvation. |
| [GroupChr](./groupchr/) | Anger grupp-teckenekvation. |
| [Matrix](./matrix/) | Anger matrisekvationen, |
| [ArrayEquation](./arrayequation/) | Anger funktionen Equation-Array. Funktionen består av en eller flera ekvationer. |

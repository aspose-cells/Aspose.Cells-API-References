---
title: "Enumeración EquationNodeType"
linktitle: "EquationNodeType"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Enumeración EquationNodeType. Encapsula el objeto que representa equationnodetype en Go."
type: docs
weight: 200
url: /es/go-cpp/equationnodetype/
---

## EquationNodeType Enum

Equation node type.Notice:(1)[1-99] Currently there is only one node in the scope, and its enumeration value is 1. The node it specifies is used to store mathematical text.(2)[100-199] Indicates that the node is a component of some special function nodes.(3)[200-] Indicates that the node has some special functions.

```go

type EquationNodeType int32


```

## Fields

| Field | Description |
| --- | --- |
| [UnKnow](./unknow/) | Desconocido |
| [Text](./text/) | especifica un nodo que almacena texto matemático |
| [Base](./base/) | Especifica un componente Base |
| [Denominator](./denominator/) | Especifica un componente Denominador |
| [Numerator](./numerator/) | Especifica un componente Numerador |
| [FunctionName](./functionname/) | Especifica un componente FunctionName |
| [Subscript](./subscript/) | Especifica un componente Subíndice |
| [Superscript](./superscript/) | Especifica un componente Superíndice |
| [Degree](./degree/) | Especifica un componente Grado |
| [MatrixRow](./matrixrow/) | Especifica un componente MatrixRow. Una única fila de la matriz |
| [Limit](./limit/) | Representa un subobjeto de la función Límite Inferior o función Límite Superior |
| [EquationParagraph](./equationparagraph/) | Especifica un párrafo matemático (oMathPara). |
| [LowerLimit](./lowerlimit/) | Especifica la función Límite Inferior |
| [UpperLimit](./upperlimit/) | Especifica la función Límite Superior |
| [Mathematical](./mathematical/) | Especifica una ecuación o expresión matemática (OMath). |
| [Fraction](./fraction/) | Especifica una ecuación fraccionaria |
| [Function](./function/) | Especifica una ecuación de función |
| [Delimiter](./delimiter/) | Especifica una ecuación delimitadora |
| [Nary](./nary/) | Especifica una ecuación de operador n-ario |
| [Radical](./radical/) | Especifica la ecuación radical |
| [Sup](./sup/) | Especifica una ecuación de superíndice |
| [Sub](./sub/) | Especifica la ecuación de subíndice |
| [SubSup](./subsup/) | Especifica una ecuación con superíndices y subíndices a la derecha de los operandos. |
| [PreSubSup](./presubsup/) | Especifica una ecuación con superíndices y subíndices a la izquierda de los operandos. |
| [Accent](./accent/) | Especifica una ecuación de acento |
| [Bar](./bar/) | Especifica una ecuación de barra |
| [BorderBox](./borderbox/) | Especifica una ecuación de cuadro con borde |
| [Box](./box/) | Especifica una ecuación de cuadro |
| [GroupChr](./groupchr/) | Especifica una ecuación Group-Character |
| [Matrix](./matrix/) | Especifica la ecuación Matrix, |
| [ArrayEquation](./arrayequation/) | Especifica la función Equation-Array. La función consta de una o más ecuaciones. |

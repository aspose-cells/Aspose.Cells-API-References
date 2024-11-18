---
title: EquationNodeType Enum 
linktitle: EquationNodeType
second_title: Aspose.Cells for Go API Reference
description: 'EquationNodeType enum. Encapsulates the object that represents equationnodetype in Go.'
type: docs
weight: 200
url: /go/aspose.cells.drawing.equations/equationnodetype/
---

## EquationNodeType Enum

Equation node type.Notice:(1)[1-99] Currently there is only one node in the scope, and its enumeration value is 1. The node it specifies is used to store mathematical text.(2)[100-199] Indicates that the node is a component of some special function nodes.(3)[200-] Indicates that the node has some special functions(Usually with 'Equation' suffix. 'EquationParagraph' is a special case.).

```go

type EquationNodeType int32


```

## Fields

| Field | Description |
| --- | --- |
|[UnKnow](./unknow/) | UnKnow | 
|[Text](./text/) | specifies a node that stores math text | 
|[Base](./base/) | Specifies a Base component | 
|[Denominator](./denominator/) | Specifies a Denominator component | 
|[Numerator](./numerator/) | Specifies a Numerator component | 
|[FunctionName](./functionname/) | Specifies a FunctionName component | 
|[Subscript](./subscript/) | Specifies a Subscript component | 
|[Superscript](./superscript/) | Specifies a Superscript component | 
|[Degree](./degree/) | Specifies a Degree component | 
|[MatrixRow](./matrixrow/) | Specifies a MatrixRow component.A single row of the matrix | 
|[Limit](./limit/) | If the parent object is limLow,the object of this type specifies the lower limit of the limLow function; if the parent objectis limUpp, the object of this type specifies the Upper-Limit function, consisting of text on the baseline and reduced-size text just above the baseline. | 
|[EquationParagraph](./equationparagraph/) | Specifies a mathematical paragraph(oMathPara). | 
|[MathematicalEquation](./mathematicalequation/) | Specifies an equation or mathematical expression(OMath). | 
|[FractionEquation](./fractionequation/) | Specifies fractional equation | 
|[FunctionEquation](./functionequation/) | Specifies function equation | 
|[DelimiterEquation](./delimiterequation/) | Specifies delimiter equation | 
|[NaryEquation](./naryequation/) | Specifies n-ary operator equation | 
|[RadicalEquation](./radicalequation/) | Specifies the radical equation | 
|[SuperscriptEquation](./superscriptequation/) | Specifies superscript equation | 
|[SubscriptEquation](./subscriptequation/) | Specifies subscript equation | 
|[SubSupEquation](./subsupequation/) | Specifies an equation with superscripts and subscripts to the right of the operands. | 
|[PreSubSupEquation](./presubsupequation/) | Specifies an equation with superscripts and subscripts to the left of the operands. | 
|[AccentEquation](./accentequation/) | Specifies accent equation | 
|[BarEquation](./barequation/) | Specifies bar equation | 
|[BorderBoxEquation](./borderboxequation/) | Specifies border box equation | 
|[BoxEquation](./boxequation/) | Specifies box equation | 
|[GroupCharacterEquation](./groupcharacterequation/) | Specifies Group-Character equation | 
|[MatrixEquation](./matrixequation/) | Specifies the Matrix equation, | 
|[LowerLimit](./lowerlimit/) | Specifies the Lower-Limit function | 
|[UpperLimit](./upperlimit/) | Specifies the Upper-Limit function | 

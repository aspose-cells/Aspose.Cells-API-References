---
title: Aspose::Cells::Drawing::Equations::EquationNodeType enum
linktitle: EquationNodeType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Equations::EquationNodeType enum. Equation node type. Notice: (1)[1-99] Currently there is only one node in the scope, and its enumeration value is 1. The node it specifies is used to store mathematical text. (2)[100-199] Indicates that the node is a component of some special function nodes. (3)[200-] Indicates that the node has some special functions(Usually with ''Equation'' suffix. ''EquationParagraph'' is a special case.) in C++.'
type: docs
weight: 2600
url: /cpp/aspose.cells.drawing.equations/equationnodetype/
---
## EquationNodeType enum


Equation node type. Notice: (1)[1-99] Currently there is only one node in the scope, and its enumeration value is 1. The node it specifies is used to store mathematical text. (2)[100-199] Indicates that the node is a component of some special function nodes. (3)[200-] Indicates that the node has some special functions(Usually with 'Equation' suffix. 'EquationParagraph' is a special case.).

```cpp
enum class EquationNodeType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| UnKnow | 0 | <br>UnKnow. |
| Text | 1 | <br>specifies a node that stores math text |
| Base | 100 | <br>Specifies a component of type 'Base'. |
| Denominator | 101 | <br>Specifies a component of type 'Denominator'. |
| Numerator | 102 | <br>Specifies a component of type 'Numerator'. |
| FunctionName | 103 | <br>Specifies a component of type 'FunctionName'. |
| Subscript | 104 | <br>Specifies a component of type 'Subscript'. |
| Superscript | 105 | <br>Specifies a component of type 'Superscript'. |
| Degree | 106 | <br>Specifies a component of type 'Degree'. |
| MatrixRow | 107 | <br>Specifies a component of type 'MatrixRow'.A single row of the matrix. |
| EquationParagraph | 200 | <br>Specifies a mathematical paragraph(oMathPara). |
| MathematicalEquation | 201 | <br>Specifies an equation or mathematical expression(OMath). |
| FractionEquation | 202 | <br>Specifies fractional equation. |
| FunctionEquation | 203 | <br>Specifies function equation. |
| DelimiterEquation | 204 | <br>Specifies delimiter equation. |
| NaryEquation | 205 | <br>Specifies n-ary operator equation. |
| RadicalEquation | 206 | <br>Specifies the radical equation. |
| SuperscriptEquation | 207 | <br>Specifies superscript equation. |
| SubscriptEquation | 208 | <br>Specifies subscript equation. |
| SubSupEquation | 209 | <br>Specifies an equation with superscripts and subscripts to the right of the operands. |
| PreSubSupEquation | 210 | <br>Specifies an equation with superscripts and subscripts to the left of the operands. |
| AccentEquation | 211 | <br>Specifies accent equation. |
| BarEquation | 212 | <br>Specifies bar equation. |
| BorderBoxEquation | 213 | <br>Specifies border box equation. |
| BoxEquation | 214 | <br>Specifies box equation. |
| GroupCharacterEquation | 215 | <br>Specifies Group-Character equation. |
| MatrixEquation | 216 | <br>Specifies the Matrix equation,. |

## See Also

* Namespace [Aspose::Cells::Drawing::Equations](../)
* Library [Aspose.Cells for C++](../../)

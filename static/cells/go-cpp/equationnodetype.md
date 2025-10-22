##EquationNodeType Enum
'EquationNodeType enum. Encapsulates the object that represents equationnodetype in Go.'
## EquationNodeType Enum
Equation node type.Notice:(1)[1-99] Currently there is only one node in the scope, and its enumeration value is 1. The node it specifies is used to store mathematical text.(2)[100-199] Indicates that the node is a component of some special function nodes.(3)[200-] Indicates that the node has some special functions.
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
|[Limit](./limit/) | Represents a sub-object of Lower-Limit function or Upper-Limit function |
|[EquationParagraph](./equationparagraph/) | Specifies a mathematical paragraph(oMathPara). |
|[LowerLimit](./lowerlimit/) | Specifies the Lower-Limit function |
|[UpperLimit](./upperlimit/) | Specifies the Upper-Limit function |
|[Mathematical](./mathematical/) | Specifies an equation or mathematical expression(OMath). |
|[Fraction](./fraction/) | Specifies fractional equation |
|[Function](./function/) | Specifies function equation |
|[Delimiter](./delimiter/) | Specifies delimiter equation |
|[Nary](./nary/) | Specifies n-ary operator equation |
|[Radical](./radical/) | Specifies the radical equation |
|[Sup](./sup/) | Specifies superscript equation |
|[Sub](./sub/) | Specifies subscript equation |
|[SubSup](./subsup/) | Specifies an equation with superscripts and subscripts to the right of the operands. |
|[PreSubSup](./presubsup/) | Specifies an equation with superscripts and subscripts to the left of the operands. |
|[Accent](./accent/) | Specifies accent equation |
|[Bar](./bar/) | Specifies bar equation |
|[BorderBox](./borderbox/) | Specifies border box equation |
|[Box](./box/) | Specifies box equation |
|[GroupChr](./groupchr/) | Specifies Group-Character equation |
|[Matrix](./matrix/) | Specifies the Matrix equation, |
|[ArrayEquation](./arrayequation/) | Specifies the Equation-Array function. The function consists of one or more equations. |

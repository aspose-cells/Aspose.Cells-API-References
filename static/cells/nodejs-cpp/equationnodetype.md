##EquationNodeType
Equation node type. Notice 1199 Currently there is only one node in the scope and its enumeration value is 1. The node it specifies is used to store mathematical text. 2100199 Indicates that the node is a component of some special function nodes. 3200 Indicates that the node has some special functions.
## EquationNodeType enumeration
Equation node type. Notice: (1)[1-99] Currently there is only one node in the scope, and its enumeration value is 1. The node it specifies is used to store mathematical text. (2)[100-199] Indicates that the node is a component of some special function nodes. (3)[200-] Indicates that the node has some special functions.
### Values
| Name | Value | Description |
| --- | --- | --- |
| UnKnow | `0` | UnKnow |
| Text | `1` | specifies a node that stores math text |
| Base | `100` | Specifies a Base component |
| Denominator | `101` | Specifies a Denominator component |
| Numerator | `102` | Specifies a Numerator component |
| FunctionName | `103` | Specifies a FunctionName component |
| Subscript | `104` | Specifies a Subscript component |
| Superscript | `105` | Specifies a Superscript component |
| Degree | `106` | Specifies a Degree component |
| MatrixRow | `107` | Specifies a MatrixRow component.A single row of the matrix |
| Limit | `108` | Represents a sub-object of Lower-Limit function or Upper-Limit function |
| EquationParagraph | `200` | Specifies a mathematical paragraph(oMathPara). |
| MathematicalEquation | `201` | Specifies an equation or mathematical expression(OMath). |
| FractionEquation | `202` | Specifies fractional equation |
| FunctionEquation | `203` | Specifies function equation |
| DelimiterEquation | `204` | Specifies delimiter equation |
| NaryEquation | `205` | Specifies n-ary operator equation |
| RadicalEquation | `206` | Specifies the radical equation |
| SuperscriptEquation | `207` | Specifies superscript equation |
| SubscriptEquation | `208` | Specifies subscript equation |
| SubSupEquation | `209` | Specifies an equation with superscripts and subscripts to the right of the operands. |
| PreSubSupEquation | `210` | Specifies an equation with superscripts and subscripts to the left of the operands. |
| AccentEquation | `211` | Specifies accent equation |
| BarEquation | `212` | Specifies bar equation |
| BorderBoxEquation | `213` | Specifies border box equation |
| BoxEquation | `214` | Specifies box equation |
| GroupCharacterEquation | `215` | Specifies Group-Character equation |
| MatrixEquation | `216` | Specifies the Matrix equation, |
| LowerLimit | `217` | Specifies the Lower-Limit function |
| UpperLimit | `218` | Specifies the Upper-Limit function |
| Mathematical | `201` | Specifies an equation or mathematical expression(OMath). |
| Fraction | `202` | Specifies fractional equation |
| Function | `203` | Specifies function equation |
| Delimiter | `204` | Specifies delimiter equation |
| Nary | `205` | Specifies n-ary operator equation |
| Radical | `206` | Specifies the radical equation |
| Sup | `207` | Specifies superscript equation |
| Sub | `208` | Specifies subscript equation |
| SubSup | `209` | Specifies an equation with superscripts and subscripts to the right of the operands. |
| PreSubSup | `210` | Specifies an equation with superscripts and subscripts to the left of the operands. |
| Accent | `211` | Specifies accent equation |
| Bar | `212` | Specifies bar equation |
| BorderBox | `213` | Specifies border box equation |
| Box | `214` | Specifies box equation |
| GroupChr | `215` | Specifies Group-Character equation |
| Matrix | `216` | Specifies the Matrix equation, |
| ArrayEquation | `317` | Specifies the Equation-Array function. The function consists of one or more equations. |

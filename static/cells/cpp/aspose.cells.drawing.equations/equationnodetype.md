##Aspose::Cells::Drawing::Equations::EquationNodeType enum
'Aspose::Cells::Drawing::Equations::EquationNodeType enum. Equation node type. Notice: (1)[1-99] Currently there is only one node in the scope, and its enumeration value is 1. The node it specifies is used to store mathematical text. (2)[100-199] Indicates that the node is a component of some special function nodes. (3)[200-] Indicates that the node has some special functions in C++.'
## EquationNodeType enum
Equation node type. Notice: (1)[1-99] Currently there is only one node in the scope, and its enumeration value is 1. The node it specifies is used to store mathematical text. (2)[100-199] Indicates that the node is a component of some special function nodes. (3)[200-] Indicates that the node has some special functions.
```cpp
enum class EquationNodeType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| UnKnow | 0 | <br>UnKnow. |
| Text | 1 | <br>specifies a node that stores math text |
| Base | 100 | <br>Specifies a Base component. |
| Denominator | 101 | <br>Specifies a Denominator component. |
| Numerator | 102 | <br>Specifies a Numerator component. |
| FunctionName | 103 | <br>Specifies a FunctionName component. |
| Subscript | 104 | <br>Specifies a Subscript component. |
| Superscript | 105 | <br>Specifies a Superscript component. |
| Degree | 106 | <br>Specifies a Degree component. |
| MatrixRow | 107 | <br>Specifies a MatrixRow component.A single row of the matrix. |
| Limit | 108 | <br>Represents a sub-object of Lower-Limit function or Upper-Limit function. |
| EquationParagraph | 200 | <br>Specifies a mathematical paragraph(oMathPara). |
| MathematicalEquation | 201 |  **(Deprecated - Use EquationNodeType.Mathematical instead. )** <br>Specifies an equation or mathematical expression(OMath). |
| FractionEquation | 202 |  **(Deprecated - Use EquationNodeType.Fraction instead. )** <br>Specifies fractional equation. |
| FunctionEquation | 203 |  **(Deprecated - Use EquationNodeType.Function instead. )** <br>Specifies function equation. |
| DelimiterEquation | 204 |  **(Deprecated - Use EquationNodeType.Delimiter instead. )** <br>Specifies delimiter equation. |
| NaryEquation | 205 |  **(Deprecated - Use EquationNodeType.Nary instead. )** <br>Specifies n-ary operator equation. |
| RadicalEquation | 206 |  **(Deprecated - Use EquationNodeType.Radical instead. )** <br>Specifies the radical equation. |
| SuperscriptEquation | 207 |  **(Deprecated - Use EquationNodeType.Sup instead. )** <br>Specifies superscript equation. |
| SubscriptEquation | 208 |  **(Deprecated - Use EquationNodeType.Sub instead. )** <br>Specifies subscript equation. |
| SubSupEquation | 209 |  **(Deprecated - Use EquationNodeType.SubSup instead. )** <br>Specifies an equation with superscripts and subscripts to the right of the operands. |
| PreSubSupEquation | 210 |  **(Deprecated - Use EquationNodeType.PreSubSup instead. )** <br>Specifies an equation with superscripts and subscripts to the left of the operands. |
| AccentEquation | 211 |  **(Deprecated - Use EquationNodeType.Accent instead. )** <br>Specifies accent equation. |
| BarEquation | 212 |  **(Deprecated - Use EquationNodeType.Bar instead. )** <br>Specifies bar equation. |
| BorderBoxEquation | 213 |  **(Deprecated - Use EquationNodeType.BorderBox instead. )** <br>Specifies border box equation. |
| BoxEquation | 214 |  **(Deprecated - Use EquationNodeType.Box instead. )** <br>Specifies box equation. |
| GroupCharacterEquation | 215 |  **(Deprecated - Use EquationNodeType.GroupChr instead. )** <br>Specifies Group-Character equation. |
| MatrixEquation | 216 |  **(Deprecated - Use EquationNodeType.Matrix instead. )** <br>Specifies the Matrix equation,. |
| LowerLimit | 217 | <br>Specifies the Lower-Limit function. |
| UpperLimit | 218 | <br>Specifies the Upper-Limit function. |
| Mathematical | 201 | <br>Specifies an equation or mathematical expression(OMath). |
| Fraction | 202 | <br>Specifies fractional equation. |
| Function | 203 | <br>Specifies function equation. |
| Delimiter | 204 | <br>Specifies delimiter equation. |
| Nary | 205 | <br>Specifies n-ary operator equation. |
| Radical | 206 | <br>Specifies the radical equation. |
| Sup | 207 | <br>Specifies superscript equation. |
| Sub | 208 | <br>Specifies subscript equation. |
| SubSup | 209 | <br>Specifies an equation with superscripts and subscripts to the right of the operands. |
| PreSubSup | 210 | <br>Specifies an equation with superscripts and subscripts to the left of the operands. |
| Accent | 211 | <br>Specifies accent equation. |
| Bar | 212 | <br>Specifies bar equation. |
| BorderBox | 213 | <br>Specifies border box equation. |
| Box | 214 | <br>Specifies box equation. |
| GroupChr | 215 | <br>Specifies Group-Character equation. |
| Matrix | 216 | <br>Specifies the Matrix equation,. |
| ArrayEquation | 317 | <br>Specifies the Equation-Array function. The function consists of one or more equations. |
## See Also
* Namespace [Aspose::Cells::Drawing::Equations](../)
* Library [Aspose.Cells for C++](../../)

##Aspose.Cells.Drawing.Equations
The Aspose.Cells.Drawing.Equations namespace provides classes for creating various equation shapes such as fractional equations power equations etc. through equation nodes
The **Aspose.Cells.Drawing.Equations** namespace provides classes for creating various equation shapes (such as fractional equations, power equations, etc.) through equation nodes.
## Classes
| Class | Description |
| --- | --- |
| [AccentEquationNode](./accentequationnode/) | This class specifies an accent equation, consisting of a base component and a combining diacritic. |
| [ArrayEquationNode](./arrayequationnode/) | Specifies the Equation-Array function, an object consisting of one or more equations. |
| [BarEquationNode](./barequationnode/) | This class specifies the bar equation, consisting of a base argument and an overbar or underbar. |
| [BorderBoxEquationNode](./borderboxequationnode/) | This class specifies the Border Box function, consisting of a border drawn around an equation. |
| [BoxEquationNode](./boxequationnode/) | This class specifies the box function, which is used to group components of an equation. |
| [DelimiterEquationNode](./delimiterequationnode/) | This class specifies the delimiter equation, consisting of opening and closing delimiters (such as parentheses, braces, brackets, and vertical bars), and a component contained inside. The delimiter may have more than one component, with a designated separator character between each component. |
| [EquationComponentNode](./equationcomponentnode/) | This class specifies the components of an equation or mathematical expression. Different types of components combined into different equations. For example, a fraction consists of two parts, a numerator component and a denominator component. For more component types, please refer to 'EquationNodeType'. |
| [EquationNode](./equationnode/) | Abstract class for deriving other equation nodes. |
| [EquationNodeParagraph](./equationnodeparagraph/) | This class specifies a mathematical paragraph containing one or more MathEquationNode(OMath) elements. |
| [FractionEquationNode](./fractionequationnode/) | This class specifies the fraction equation, consisting of a numerator and denominator separated by a fraction bar. The fraction bar can be horizontal or diagonal, depending on the fraction properties. The fraction equation is also used to represent the stack function, which places one element above another, with no fraction bar. |
| [FunctionEquationNode](./functionequationnode/) | This class specifies the Function-Apply equation, which consists of a function name and an argument acted upon. The types of the name and argument components are 'EquationNodeType.FunctionName' and 'EquationNodeType.Base' respectively. |
| [GroupCharacterEquationNode](./groupcharacterequationnode/) | This class specifies the Group-Character function, consisting of a character drawn above or below text, often with the purpose of visually grouping items. |
| [LimLowUppEquationNode](./limlowuppequationnode/) | This class specifies the limit function. |
| [MathematicalEquationNode](./mathematicalequationnode/) | This class specifies an equation or mathematical expression. All mathematical text of equations or mathematical expressions are contained by this class. |
| [MatrixEquationNode](./matrixequationnode/) | This class specifies the Matrix equation, consisting of one or more elements laid out in one or more rows and one or more columns. |
| [NaryEquationNode](./naryequationnode/) | This class specifies an n-ary operator equation consisting of an n-ary operator, a base (or operand), and optional upper and lower bounds. |
| [RadicalEquationNode](./radicalequationnode/) | This class specifies the radical equation, consisting of an optional degree deg(EquationNodeType.Degree) and a base. |
| [SubSupEquationNode](./subsupequationnode/) | This class specifies an equation that can optionally be superscript or subscript. There are four main forms of this equation, superscript，subscript，superscript and subscript placed to the left of the base, superscript and subscript placed to the right of the base. |
| [TextRunEquationNode](./textrunequationnode/) | This class in the equation node is used to store the actual content(a sequence of mathematical text) of the equation. Usually a node object per character. |
| [UnknowEquationNode](./unknowequationnode/) | Equation node class of unknown type |
## Enumeration
| Enumeration | Description |
| --- | --- |
| [EquationCharacterPositionType](./equationcharacterpositiontype/) | Specifies the position of a particular subobject within its parent |
| [EquationCombiningCharacterType](./equationcombiningcharactertype/) | Type of combining characters. |
| [EquationDelimiterShapeType](./equationdelimitershapetype/) | This specifies the shape of delimiters in the delimiter object. |
| [EquationFractionType](./equationfractiontype/) | This specifies the display style of the fraction bar. |
| [EquationHorizontalJustificationType](./equationhorizontaljustificationtype/) | This specifies the default horizontal justification of equations in the document. |
| [EquationLimitLocationType](./equationlimitlocationtype/) | Specifies the limit location on an operator. |
| [EquationMathematicalOperatorType](./equationmathematicaloperatortype/) | Mathematical Operators Type |
| [EquationNodeType](./equationnodetype/) | Equation node type. Notice: (1)[1-99] Currently there is only one node in the scope, and its enumeration value is 1. The node it specifies is used to store mathematical text. (2)[100-199] Indicates that the node is a component of some special function nodes. (3)[200-] Indicates that the node has some special functions. |
| [EquationVerticalJustificationType](./equationverticaljustificationtype/) | This specifies the default vertical justification of equations in the document. |

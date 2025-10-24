##EquationNodeType
Equation node type.
**Inheritance:**
java.lang.Object
```
public final class EquationNodeType
```
Equation node type. Notice: (1)[1-99] Currently there is only one node in the scope, and its enumeration value is 1. The node it specifies is used to store mathematical text. (2)[100-199] Indicates that the node is a component of some special function nodes. (3)[200-] Indicates that the node has some special functions.
## Fields
| Field | Description |
| --- | --- |
| [ACCENT](#ACCENT) | Specifies accent equation |
| [ACCENT_EQUATION](#ACCENT-EQUATION) | Specifies accent equation |
| [ARRAY_EQUATION](#ARRAY-EQUATION) | Specifies the Equation-Array function. |
| [BAR](#BAR) | Specifies bar equation |
| [BAR_EQUATION](#BAR-EQUATION) | Specifies bar equation |
| [BASE](#BASE) | Specifies a Base component |
| [BORDER_BOX](#BORDER-BOX) | Specifies border box equation |
| [BORDER_BOX_EQUATION](#BORDER-BOX-EQUATION) | Specifies border box equation |
| [BOX](#BOX) | Specifies box equation |
| [BOX_EQUATION](#BOX-EQUATION) | Specifies box equation |
| [DEGREE](#DEGREE) | Specifies a Degree component |
| [DELIMITER](#DELIMITER) | Specifies delimiter equation |
| [DELIMITER_EQUATION](#DELIMITER-EQUATION) | Specifies delimiter equation |
| [DENOMINATOR](#DENOMINATOR) | Specifies a Denominator component |
| [EQUATION_PARAGRAPH](#EQUATION-PARAGRAPH) | Specifies a mathematical paragraph(oMathPara). |
| [FRACTION](#FRACTION) | Specifies fractional equation |
| [FRACTION_EQUATION](#FRACTION-EQUATION) | Specifies fractional equation |
| [FUNCTION](#FUNCTION) | Specifies function equation |
| [FUNCTION_EQUATION](#FUNCTION-EQUATION) | Specifies function equation |
| [FUNCTION_NAME](#FUNCTION-NAME) | Specifies a FunctionName component |
| [GROUP_CHARACTER_EQUATION](#GROUP-CHARACTER-EQUATION) | Specifies Group-Character equation |
| [GROUP_CHR](#GROUP-CHR) | Specifies Group-Character equation |
| [LIMIT](#LIMIT) | Represents a sub-object of Lower-Limit function or Upper-Limit function |
| [LOWER_LIMIT](#LOWER-LIMIT) | Specifies the Lower-Limit function |
| [MATHEMATICAL](#MATHEMATICAL) | Specifies an equation or mathematical expression(OMath). |
| [MATHEMATICAL_EQUATION](#MATHEMATICAL-EQUATION) | Specifies an equation or mathematical expression(OMath). |
| [MATRIX](#MATRIX) | Specifies the Matrix equation, |
| [MATRIX_EQUATION](#MATRIX-EQUATION) | Specifies the Matrix equation, |
| [MATRIX_ROW](#MATRIX-ROW) | Specifies a MatrixRow component.A single row of the matrix |
| [NARY](#NARY) | Specifies n-ary operator equation |
| [NARY_EQUATION](#NARY-EQUATION) | Specifies n-ary operator equation |
| [NUMERATOR](#NUMERATOR) | Specifies a Numerator component |
| [PRE_SUB_SUP](#PRE-SUB-SUP) | Specifies an equation with superscripts and subscripts to the left of the operands. |
| [PRE_SUB_SUP_EQUATION](#PRE-SUB-SUP-EQUATION) | Specifies an equation with superscripts and subscripts to the left of the operands. |
| [RADICAL](#RADICAL) | Specifies the radical equation |
| [RADICAL_EQUATION](#RADICAL-EQUATION) | Specifies the radical equation |
| [SUB](#SUB) | Specifies subscript equation |
| [SUBSCRIPT](#SUBSCRIPT) | Specifies a Subscript component |
| [SUBSCRIPT_EQUATION](#SUBSCRIPT-EQUATION) | Specifies subscript equation |
| [SUB_SUP](#SUB-SUP) | Specifies an equation with superscripts and subscripts to the right of the operands. |
| [SUB_SUP_EQUATION](#SUB-SUP-EQUATION) | Specifies an equation with superscripts and subscripts to the right of the operands. |
| [SUP](#SUP) | Specifies superscript equation |
| [SUPERSCRIPT](#SUPERSCRIPT) | Specifies a Superscript component |
| [SUPERSCRIPT_EQUATION](#SUPERSCRIPT-EQUATION) | Specifies superscript equation |
| [TEXT](#TEXT) | specifies a node that stores math text |
| [UN_KNOW](#UN-KNOW) | UnKnow |
| [UPPER_LIMIT](#UPPER-LIMIT) | Specifies the Upper-Limit function |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ACCENT {#ACCENT}
```
public static final int ACCENT
```
Specifies accent equation
### ACCENT_EQUATION {#ACCENT-EQUATION}
```
public static final int ACCENT_EQUATION
```
Specifies accent equation
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.Accent. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### ARRAY_EQUATION {#ARRAY-EQUATION}
```
public static final int ARRAY_EQUATION
```
Specifies the Equation-Array function. The function consists of one or more equations.
### BAR {#BAR}
```
public static final int BAR
```
Specifies bar equation
### BAR_EQUATION {#BAR-EQUATION}
```
public static final int BAR_EQUATION
```
Specifies bar equation
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.Bar. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### BASE {#BASE}
```
public static final int BASE
```
Specifies a Base component
### BORDER_BOX {#BORDER-BOX}
```
public static final int BORDER_BOX
```
Specifies border box equation
### BORDER_BOX_EQUATION {#BORDER-BOX-EQUATION}
```
public static final int BORDER_BOX_EQUATION
```
Specifies border box equation
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.BorderBox. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### BOX {#BOX}
```
public static final int BOX
```
Specifies box equation
### BOX_EQUATION {#BOX-EQUATION}
```
public static final int BOX_EQUATION
```
Specifies box equation
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.Box. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### DEGREE {#DEGREE}
```
public static final int DEGREE
```
Specifies a Degree component
### DELIMITER {#DELIMITER}
```
public static final int DELIMITER
```
Specifies delimiter equation
### DELIMITER_EQUATION {#DELIMITER-EQUATION}
```
public static final int DELIMITER_EQUATION
```
Specifies delimiter equation
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.Delimiter. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### DENOMINATOR {#DENOMINATOR}
```
public static final int DENOMINATOR
```
Specifies a Denominator component
### EQUATION_PARAGRAPH {#EQUATION-PARAGRAPH}
```
public static final int EQUATION_PARAGRAPH
```
Specifies a mathematical paragraph(oMathPara).
### FRACTION {#FRACTION}
```
public static final int FRACTION
```
Specifies fractional equation
### FRACTION_EQUATION {#FRACTION-EQUATION}
```
public static final int FRACTION_EQUATION
```
Specifies fractional equation
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.Fraction. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### FUNCTION {#FUNCTION}
```
public static final int FUNCTION
```
Specifies function equation
### FUNCTION_EQUATION {#FUNCTION-EQUATION}
```
public static final int FUNCTION_EQUATION
```
Specifies function equation
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.Function. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### FUNCTION_NAME {#FUNCTION-NAME}
```
public static final int FUNCTION_NAME
```
Specifies a FunctionName component
### GROUP_CHARACTER_EQUATION {#GROUP-CHARACTER-EQUATION}
```
public static final int GROUP_CHARACTER_EQUATION
```
Specifies Group-Character equation
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.GroupChr. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### GROUP_CHR {#GROUP-CHR}
```
public static final int GROUP_CHR
```
Specifies Group-Character equation
### LIMIT {#LIMIT}
```
public static final int LIMIT
```
Represents a sub-object of Lower-Limit function or Upper-Limit function
### LOWER_LIMIT {#LOWER-LIMIT}
```
public static final int LOWER_LIMIT
```
Specifies the Lower-Limit function
### MATHEMATICAL {#MATHEMATICAL}
```
public static final int MATHEMATICAL
```
Specifies an equation or mathematical expression(OMath).
### MATHEMATICAL_EQUATION {#MATHEMATICAL-EQUATION}
```
public static final int MATHEMATICAL_EQUATION
```
Specifies an equation or mathematical expression(OMath).
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.Mathematical. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### MATRIX {#MATRIX}
```
public static final int MATRIX
```
Specifies the Matrix equation,
### MATRIX_EQUATION {#MATRIX-EQUATION}
```
public static final int MATRIX_EQUATION
```
Specifies the Matrix equation,
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.Matrix. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### MATRIX_ROW {#MATRIX-ROW}
```
public static final int MATRIX_ROW
```
Specifies a MatrixRow component.A single row of the matrix
### NARY {#NARY}
```
public static final int NARY
```
Specifies n-ary operator equation
### NARY_EQUATION {#NARY-EQUATION}
```
public static final int NARY_EQUATION
```
Specifies n-ary operator equation
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.Nary. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### NUMERATOR {#NUMERATOR}
```
public static final int NUMERATOR
```
Specifies a Numerator component
### PRE_SUB_SUP {#PRE-SUB-SUP}
```
public static final int PRE_SUB_SUP
```
Specifies an equation with superscripts and subscripts to the left of the operands.
### PRE_SUB_SUP_EQUATION {#PRE-SUB-SUP-EQUATION}
```
public static final int PRE_SUB_SUP_EQUATION
```
Specifies an equation with superscripts and subscripts to the left of the operands.
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.PreSubSup. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### RADICAL {#RADICAL}
```
public static final int RADICAL
```
Specifies the radical equation
### RADICAL_EQUATION {#RADICAL-EQUATION}
```
public static final int RADICAL_EQUATION
```
Specifies the radical equation
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.Radical. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### SUB {#SUB}
```
public static final int SUB
```
Specifies subscript equation
### SUBSCRIPT {#SUBSCRIPT}
```
public static final int SUBSCRIPT
```
Specifies a Subscript component
### SUBSCRIPT_EQUATION {#SUBSCRIPT-EQUATION}
```
public static final int SUBSCRIPT_EQUATION
```
Specifies subscript equation
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.Sub. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### SUB_SUP {#SUB-SUP}
```
public static final int SUB_SUP
```
Specifies an equation with superscripts and subscripts to the right of the operands.
### SUB_SUP_EQUATION {#SUB-SUP-EQUATION}
```
public static final int SUB_SUP_EQUATION
```
Specifies an equation with superscripts and subscripts to the right of the operands.
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.SubSup. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### SUP {#SUP}
```
public static final int SUP
```
Specifies superscript equation
### SUPERSCRIPT {#SUPERSCRIPT}
```
public static final int SUPERSCRIPT
```
Specifies a Superscript component
### SUPERSCRIPT_EQUATION {#SUPERSCRIPT-EQUATION}
```
public static final int SUPERSCRIPT_EQUATION
```
Specifies superscript equation
**Remarks**
NOTE: This member is now obsolete. Instead, please use EquationNodeType.Sup. This property will be removed 12 months later since September 2024. Aspose apologizes for any inconvenience you may have experienced.
### TEXT {#TEXT}
```
public static final int TEXT
```
specifies a node that stores math text
### UN_KNOW {#UN-KNOW}
```
public static final int UN_KNOW
```
UnKnow
### UPPER_LIMIT {#UPPER-LIMIT}
```
public static final int UPPER_LIMIT
```
Specifies the Upper-Limit function
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

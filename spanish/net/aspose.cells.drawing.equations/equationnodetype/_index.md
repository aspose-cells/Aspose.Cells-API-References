---
title: "Enumeración EquationNodeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.Equations.EquationNodeType. Tipo de nodo de ecuación. Nota 1199 Actualmente solo hay un nodo en el alcance y su valor de enumeración es 1. El nodo que especifica se usa para almacenar texto matemático. 2100199 Indica que el nodo es un componente de algunos nodos de funciones especiales. 3200 Indica que el nodo tiene algunas funciones especiales"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnodetype/
---
## EquationNodeType enumeration

Tipo de nodo de ecuación. Nota: (1)[1-99] Actualmente solo hay un nodo en el alcance, y su valor de enumeración es 1. El nodo que especifica se usa para almacenar texto matemático. (2)[100-199] Indica que el nodo es un componente de algunos nodos de funciones especiales. (3)[200-] Indica que el nodo tiene algunas funciones especiales.

```csharp
public enum EquationNodeType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| UnKnow | `0` | Desconocido |
| Text | `1` | especifica un nodo que almacena texto matemático |
| Base | `100` | Especifica un componente Base |
| Denominator | `101` | Especifica un componente Denominator |
| Numerator | `102` | Especifica un componente Numerator |
| FunctionName | `103` | Especifica un componente FunctionName |
| Subscript | `104` | Especifica un componente Subscript |
| Superscript | `105` | Especifica un componente Superscript |
| Degree | `106` | Especifica un componente Degree |
| MatrixRow | `107` | Especifica un componente MatrixRow. Una única fila de la matriz |
| Limit | `108` | Representa un subobjeto de la función Lower-Limit o Upper-Limit |
| EquationParagraph | `200` | Especifica un párrafo matemático(oMathPara). |
| MathematicalEquation | `201` | Especifica una ecuación o expresión matemática(OMath). |
| FractionEquation | `202` | Especifica una ecuación fraccionaria |
| FunctionEquation | `203` | Especifica una ecuación de función |
| DelimiterEquation | `204` | Especifica una ecuación delimitadora |
| NaryEquation | `205` | Especifica una ecuación de operador n-ario |
| RadicalEquation | `206` | Especifica la ecuación radical |
| SuperscriptEquation | `207` | Especifica una ecuación en superíndice |
| SubscriptEquation | `208` | Especifica una ecuación en subíndice |
| SubSupEquation | `209` | Especifica una ecuación con superíndices y subíndices a la derecha de los operandos. |
| PreSubSupEquation | `210` | Especifica una ecuación con superíndices y subíndices a la izquierda de los operandos. |
| AccentEquation | `211` | Especifica una ecuación de acento |
| BarEquation | `212` | Especifica una ecuación de barra |
| BorderBoxEquation | `213` | Especifica una ecuación de cuadro con borde |
| BoxEquation | `214` | Especifica una ecuación de cuadro |
| GroupCharacterEquation | `215` | Especifica una ecuación de grupo de caracteres |
| MatrixEquation | `216` | Especifica la ecuación de matriz, |
| LowerLimit | `217` | Especifica la función de límite inferior |
| UpperLimit | `218` | Especifica la función de límite superior |
| Mathematical | `201` | Especifica una ecuación o expresión matemática(OMath). |
| Fraction | `202` | Especifica una ecuación fraccionaria |
| Function | `203` | Especifica una ecuación de función |
| Delimiter | `204` | Especifica una ecuación delimitadora |
| Nary | `205` | Especifica una ecuación de operador n-ario |
| Radical | `206` | Especifica la ecuación radical |
| Sup | `207` | Especifica una ecuación en superíndice |
| Sub | `208` | Especifica una ecuación en subíndice |
| SubSup | `209` | Especifica una ecuación con superíndices y subíndices a la derecha de los operandos. |
| PreSubSup | `210` | Especifica una ecuación con superíndices y subíndices a la izquierda de los operandos. |
| Accent | `211` | Especifica una ecuación de acento |
| Bar | `212` | Especifica una ecuación de barra |
| BorderBox | `213` | Especifica una ecuación de cuadro con borde |
| Box | `214` | Especifica una ecuación de cuadro |
| GroupChr | `215` | Especifica una ecuación de grupo de caracteres |
| Matrix | `216` | Especifica la ecuación de matriz, |
| ArrayEquation | `317` | Especifica la función de matriz de ecuaciones. La función consta de una o más ecuaciones. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una ecuación a la primera hoja de cálculo
            var equationShape = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtén el nodo matemático de la ecuación
            EquationNode mathNode = equationShape.GetEquationParagraph().GetChild(0);

            // Crea un nodo de acento con carácter circunflejo
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            accentNode.AccentCharacter = "\u0302";

            // Añade nodo base y nodo de texto
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // Guarda el libro de trabajo
            workbook.Save("EquationNodeTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)



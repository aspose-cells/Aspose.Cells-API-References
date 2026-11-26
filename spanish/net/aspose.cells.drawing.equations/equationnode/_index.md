---
title: "Clase EquationNode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Equations.EquationNode. Clase abstracta para derivar otros nodos de ecuación"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnode/
---
## EquationNode class

Clase abstracta para derivar otros nodos de ecuación.

```csharp
public abstract class EquationNode : FontSetting
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Obtener el tipo de ecuación del nodo actual |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Devuelve la fuente de este objeto. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Obtiene la longitud de los caracteres. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Especifica el nodo padre del nodo actual |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Obtiene el índice de inicio de los caracteres. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Devuelve las opciones de texto. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Representa el tipo del nodo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [CreateNode](../../aspose.cells.drawing.equations/equationnode/createnode/)(EquationNodeType, Workbook, EquationNode) | Crear un nodo del tipo especificado. |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/#addchild_1)(EquationNode) | Inserta el nodo especificado al final de la lista de nodos hijos del nodo actual. |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/#addchild)(EquationNodeType) | Insertar un nodo del tipo especificado al final de la lista de nodos hijos del nodo actual. |
| override [Equals](../../aspose.cells.drawing.equations/equationnode/equals/)(object) | Determinar si el nodo de ecuación actual es igual al nodo especificado |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Devuelve el nodo en el índice especificado entre los hijos del nodo actual. |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Inserta el nodo especificado después del nodo actual. |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Inserta el nodo especificado antes del nodo actual. |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Inserta un nodo del tipo especificado en la posición de índice especificada en la lista de nodos hijos del nodo actual. |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Se elimina a sí mismo del padre. |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Elimina todos los nodos hijos del nodo actual. |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/#removechild)(EquationNode) | Elimina el nodo especificado de los hijos del nodo actual. |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/#removechild_1)(int) | Elimina el nodo en el índice especificado de los hijos del nodo actual. |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Establece el estilo WordArt predefinido.(Hereda de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Convertir esta ecuación a expresión LaTeX. |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Convertir esta ecuación a expresión MathML. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationNodeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un cuadro de texto a la hoja de cálculo y obtener su índice
            int textBoxIndex = worksheet.TextBoxes.Add(10, 10, 200, 100);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "=A1+B1";
            
            // Obtener el nodo de ecuación del cuadro de texto
            EquationNode node = textBox.GetEquationParagraph();
            
            // Mostrar el texto de la ecuación usando ToString()
            Console.WriteLine("Equation: " + node.ToString());
            
            // Modificar la ecuación estableciendo nuevo texto
            textBox.Text = "=A1*B1";
            Console.WriteLine("Modified Equation: " + textBox.Text);
        }
    }
}
```

### Ver también

* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)



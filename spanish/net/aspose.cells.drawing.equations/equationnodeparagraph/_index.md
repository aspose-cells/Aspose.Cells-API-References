---
title: "Clase EquationNodeParagraph"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.Equations.EquationNodeParagraph class. Esta clase especifica un párrafo matemático que contiene uno o más elementos MathEquationNodeOMath"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnodeparagraph/
---
## EquationNodeParagraph class

Esta clase especifica un párrafo matemático que contiene uno o más elementos MathEquationNode(OMath).

```csharp
public class EquationNodeParagraph : EquationNode
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Obtener el tipo de ecuación del nodo actual (Heredado de [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Devuelve la fuente de este objeto. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Justification](../../aspose.cells.drawing.equations/equationnodeparagraph/justification/) { get; set; } | Esto especifica la justificación del párrafo matemático (una serie de ecuaciones adyacentes dentro del mismo párrafo). Un párrafo matemático puede estar alineado a la izquierda, alineado a la derecha, centrado, o centrado como grupo. Por defecto, el párrafo matemático está centrado como grupo. Esto significa que las ecuaciones pueden alinearse entre sí, pero todo el conjunto de ecuaciones está centrado en su totalidad. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Obtiene la longitud de los caracteres. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Especifica el nodo padre del nodo actual (Heredado de [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Obtiene el índice de inicio de los caracteres. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Devuelve las opciones de texto. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Representa el tipo del nodo. (Heredado de [`EquationNode`](../equationnode/).) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Inserta el nodo especificado al final de la lista de nodos hijos del nodo actual. (Heredado de [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Insertar un nodo del tipo especificado al final de la lista de nodos hijos del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/equationnodeparagraph/equals/)(object) | Determinar si el nodo de ecuación actual es igual al nodo especificado |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Devuelve el nodo en el índice especificado entre los hijos del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Inserta el nodo especificado después del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Inserta el nodo especificado antes del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Inserta un nodo del tipo especificado en la posición de índice especificado en la lista de nodos hijos del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Se elimina a sí mismo del padre.(Hereda de [`EquationNode`](../equationnode/).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Elimina todos los nodos hijos del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | Elimina el nodo especificado de los hijos del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | Elimina el nodo en el índice especificado de los hijos del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Establece el estilo WordArt predefinido.(Hereda de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Convertir esta ecuación a expresión LaTeX.(Hereda de [`EquationNode`](../equationnode/).) |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Convertir esta ecuación a expresión MathML.(Hereda de [`EquationNode`](../equationnode/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationNodeParagraphDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crear una forma para contener el párrafo de la ecuación
                var shape = worksheet.Shapes.AddTextBox(0, 0, 200, 50, 200, 50);

                // Obtener el párrafo de la ecuación desde la forma
                var equationParagraph = shape.GetEquationParagraph() as EquationNodeParagraph;

                if (equationParagraph != null)
                {
                    // Mostrar la justificación predeterminada
                    Console.WriteLine($"Default Justification: {equationParagraph.Justification}");

                    // Cambiar la justificación a la izquierda
                    equationParagraph.Justification = EquationHorizontalJustificationType.Left;
                    Console.WriteLine($"Justification changed to: {equationParagraph.Justification}");

                    // Cambiar la justificación a Centro
                    equationParagraph.Justification = EquationHorizontalJustificationType.Center;
                    Console.WriteLine($"Justification changed to: {equationParagraph.Justification}");

                    // Guarda el libro de trabajo
                    workbook.Save("EquationNodeParagraphDemo.xlsx");
                    Console.WriteLine("Workbook saved successfully.");
                }
                else
                {
                    Console.WriteLine("Failed to get EquationNodeParagraph from shape.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with EquationNodeParagraph: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)



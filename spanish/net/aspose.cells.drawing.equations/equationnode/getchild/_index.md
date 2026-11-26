---
title: "EquationNode.GetChild"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método EquationNode. Devuelve el nodo en el índice especificado entre los hijos del nodo actual"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnode/getchild/
---
## EquationNode.GetChild method

Devuelve el nodo en el índice especificado entre los hijos del nodo actual.

```csharp
public EquationNode GetChild(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | Índice del nodo |

### Valor de retorno

Devuelve el nodo correspondiente si el nodo especificado existe, de lo contrario devuelve null.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationNodeMethodGetChildWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una forma de ecuación a la primera hoja de cálculo
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
            
            // Obtén el párrafo de la ecuación y su primer nodo hijo
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Añade un nodo delimitador como hijo
            DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";
            
            // Añade un nodo de fracción dentro del delimitador
            EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            FractionEquationNode fractionNode = (FractionEquationNode)baseNode.AddChild(EquationNodeType.Fraction);
            
            // Añade numerador y denominador
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode textNode = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            textNode.Text = "X";
            
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            textNode = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            textNode.Text = "Y";
            
            // Guarda el libro de trabajo
            workbook.Save("EquationNodeGetChildDemo.xlsx");
            
            // Cargar el archivo guardado para verificar
            Workbook loadedWorkbook = new Workbook("EquationNodeGetChildDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Demostrar el método GetChild
            EquationNode loadedMathNode = loadedTextBox.GetEquationParagraph().GetChild(0);
            DelimiterEquationNode loadedDelimiter = (DelimiterEquationNode)loadedMathNode.GetChild(0);
            
            Console.WriteLine("Delimiter BeginChar: " + loadedDelimiter.BeginChar);
            Console.WriteLine("Delimiter EndChar: " + loadedDelimiter.EndChar);
            
            EquationNode loadedBaseNode = loadedDelimiter.GetChild(0);
            FractionEquationNode loadedFraction = (FractionEquationNode)loadedBaseNode.GetChild(0);
            
            Console.WriteLine("Fraction node type: " + loadedFraction.EquationType);
        }
    }
}
```

### Ver también

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



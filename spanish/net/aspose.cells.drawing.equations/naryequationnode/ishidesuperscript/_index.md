---
title: "NaryEquationNode.IsHideSuperscript"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad NaryEquationNode. Indica si se muestra el límite superior"
type: docs
url: /es/net/aspose.cells.drawing.equations/naryequationnode/ishidesuperscript/
---
## NaryEquationNode.IsHideSuperscript property

Si se muestra el límite superior

```csharp
public bool IsHideSuperscript { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyIsHideSuperscriptDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Crear un nodo de ecuación nary con superíndice oculto
            NaryEquationNode node = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            node.NaryOperator = "∫";
            node.IsHideSuperscript = true; // Demonstrating the IsHideSuperscript property
            
            // Agregar componente base
            EquationNode baseNode = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x";
            
            // Agregar superíndice (se ocultará debido a IsHideSuperscript = true)
            EquationNode supNode = node.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)supNode.AddChild(EquationNodeType.Text);
            supText.Text = "2";

            // Guardar y recargar para verificar que el superíndice está oculto
            workbook.Save("NaryEquationDemo.xlsx");
            workbook = new Workbook("NaryEquationDemo.xlsx");
            
            // Verificar la ecuación guardada
            TextBox savedTextBox = (TextBox)workbook.Worksheets[0].Shapes[0];
            EquationNode savedMathNode = savedTextBox.GetEquationParagraph().GetChild(0);
            NaryEquationNode savedNode = (NaryEquationNode)savedMathNode.GetChild(0);
            
            Console.WriteLine("Nary Operator: " + savedNode.NaryOperator);
            Console.WriteLine("IsHideSuperscript: " + savedNode.IsHideSuperscript);
            Console.WriteLine("Superscript exists: " + (savedNode.GetChild(1).GetChild(0) != null));
        }
    }
}
```

### Ver también

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



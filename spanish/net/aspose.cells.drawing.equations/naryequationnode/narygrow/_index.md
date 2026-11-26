---
title: "NaryEquationNode.NaryGrow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad NaryEquationNode. Este atributo especifica la propiedad de crecimiento de los operadores n-arios a nivel de documento. Cuando está desactivado, los operadores n-arios como integrales y sumas no crecen para coincidir con el tamaño de la altura de su operando. Cuando está activado, el operador n-ario crece verticalmente para coincidir con la altura de su operando"
type: docs
url: /es/net/aspose.cells.drawing.equations/naryequationnode/narygrow/
---
## NaryEquationNode.NaryGrow property

Este atributo especifica la propiedad de crecimiento de los operadores n-arios a nivel de documento. Cuando está desactivado, los operadores n-arios como integrales y sumas no crecen para coincidir con la altura de su operando. Cuando está activado, el operador n-ario crece verticalmente para coincidir con la altura de su operando.

```csharp
public bool NaryGrow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyNaryGrowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar forma de ecuación
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Obtener el nodo de ecuación
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Crea un nodo de operador n-ario con la propiedad NaryGrow establecida en true
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            naryNode.NaryOperator = "∑";
            naryNode.NaryGrow = true; // This is the key property we're demonstrating
            
            // Agregar subíndice (opcional)
            EquationNode sub = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subText = (TextRunEquationNode)sub.AddChild(EquationNodeType.Text);
            subText.Text = "i=1";
            
            // Agregar superíndice (opcional)
            EquationNode sup = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)sup.AddChild(EquationNodeType.Text);
            supText.Text = "n";
            
            // Agregar base (requerido)
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";
            
            // Guarda el libro de trabajo
            workbook.Save("NaryGrowDemo.xlsx");
            
            Console.WriteLine("Equation with NaryGrow property created successfully.");
        }
    }
}
```

### Ver también

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



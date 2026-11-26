---
title: "GroupCharacterEquationNode.Position"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GroupCharacterEquationNode. Este atributo especifica la posición del carácter en el objeto"
type: docs
url: /es/net/aspose.cells.drawing.equations/groupcharacterequationnode/position/
---
## GroupCharacterEquationNode.Position property

Este atributo especifica la posición del carácter en el objeto

```csharp
public EquationCharacterPositionType Position { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class GroupCharacterEquationNodePropertyPositionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una forma de ecuación a la primera hoja de cálculo
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtener el párrafo de la ecuación y agregar un nodo de carácter de grupo
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            GroupCharacterEquationNode groupNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            
            // Establecer la propiedad de posición (demostración principal)
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Agregar texto base
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "abc";

            // Guarda el libro de trabajo
            string outputPath = "GroupCharacterEquationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Equation with group character position set to Top has been created successfully.");
        }
    }
}
```

### Ver también

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



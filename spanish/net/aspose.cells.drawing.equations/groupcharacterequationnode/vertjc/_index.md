---
title: "GroupCharacterEquationNode.VertJc"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GroupCharacterEquationNode. Este atributo, combinado con pos de groupChrPr, especifica el diseño vertical del objeto groupChr. Donde pos indica la posición del carácter de agrupación, vertJc especifica la alineación del objeto con respecto a la línea base."
type: docs
url: /es/net/aspose.cells.drawing.equations/groupcharacterequationnode/vertjc/
---
## GroupCharacterEquationNode.VertJc property

Este atributo, combinado con pos de groupChrPr, especifica la disposición vertical del objeto groupChr. Donde pos indica la posición del carácter de agrupación, vertJc indica la alineación del objeto con respecto a la línea base.

```csharp
public EquationCharacterPositionType VertJc { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class GroupCharacterEquationNodePropertyVertJcDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma de cuadro de texto para contener la ecuación
            var shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            
            // Crear una instancia de GroupCharacterEquationNode
            var equationNode = (GroupCharacterEquationNode)shape.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            
            try
            {
                // Establecer propiedades iniciales para el nodo de ecuación
                equationNode.GroupChr = "⏟";
                equationNode.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
                equationNode.Position = EquationCharacterPositionType.Bottom;
                
                // Demostrar la propiedad VertJc (lectura y escritura)
                Console.WriteLine("Initial VertJc value: " + equationNode.VertJc);
                
                // Cambiar el valor de VertJc
                equationNode.VertJc = EquationCharacterPositionType.Top;
                Console.WriteLine("Modified VertJc value: " + equationNode.VertJc);
                
                // Guarda el libro de trabajo
                workbook.Save("VertJcDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



---
title: "BarEquationNode.BarPosition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BarEquationNode. Este atributo especifica la posición de la barra en el objeto barra"
type: docs
url: /es/net/aspose.cells.drawing.equations/barequationnode/barposition/
---
## BarEquationNode.BarPosition property

Este atributo especifica la posición de la barra en el objeto barra

```csharp
public EquationCharacterPositionType BarPosition { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class BarEquationNodePropertyBarPositionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una forma de ecuación a la primera hoja de cálculo
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtener el nodo de ecuación
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Crea un nodo de ecuación de barra
            BarEquationNode barNode = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
            
            // Establece la posición de la barra a Top
            barNode.BarPosition = EquationCharacterPositionType.Top;

            // Agrega contenido base para la barra
            EquationNode baseNode = barNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // Guarda el libro de trabajo
            workbook.Save("BarEquationDemo.xlsx");

            // Verifique el archivo guardado
            Workbook verifyWorkbook = new Workbook("BarEquationDemo.xlsx");
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            BarEquationNode verifyBarNode = (BarEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Bar Position: " + verifyBarNode.BarPosition);
            Console.WriteLine("Base Content: " + ((TextRunEquationNode)verifyBarNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### Ver también

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



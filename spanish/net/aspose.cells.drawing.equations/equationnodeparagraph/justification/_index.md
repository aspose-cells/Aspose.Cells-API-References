---
title: "EquationNodeParagraph.Justification"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad EquationNodeParagraph. Esto especifica la justificación del párrafo matemático, una serie de ecuaciones adyacentes dentro del mismo párrafo. Un párrafo matemático puede estar Justificado a la Izquierda, Justificado a la Derecha, Centrado o Centrado como Grupo. Por defecto, el párrafo matemático está Centrado como Grupo. Esto significa que las ecuaciones pueden alinearse entre sí, pero todo el grupo de ecuaciones está centrado como un todo"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnodeparagraph/justification/
---
## EquationNodeParagraph.Justification property

Esto especifica la justificación del párrafo matemático (una serie de ecuaciones adyacentes dentro del mismo párrafo). Un párrafo matemático puede estar alineado a la izquierda, alineado a la derecha, centrado, o centrado como grupo. Por defecto, el párrafo matemático está centrado como grupo. Esto significa que las ecuaciones pueden alinearse entre sí, pero todo el conjunto de ecuaciones está centrado en su totalidad.

```csharp
public EquationHorizontalJustificationType Justification { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeParagraphPropertyJustificationDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma para contener la ecuación
            var shape = worksheet.Shapes.AddTextBox(0, 0, 200, 50, 200, 50);

            // Obtener el párrafo de la ecuación
            var equationParagraph = shape.GetEquationParagraph() as EquationNodeParagraph;

            // Mostrar el valor de justificación actual
            Console.WriteLine("Current Justification value: " + equationParagraph.Justification);

            // Establecer diferentes valores de justificación y observar los efectos
            equationParagraph.Justification = EquationHorizontalJustificationType.Left;
            Console.WriteLine("Set to Left justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Center;
            Console.WriteLine("Set to Center justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.CenterGroup;
            Console.WriteLine("Set to CenterGroup justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Right;
            Console.WriteLine("Set to Right justification");

            // Guarda el libro de trabajo
            workbook.Save("EquationJustificationDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [EquationHorizontalJustificationType](../../equationhorizontaljustificationtype/)
* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



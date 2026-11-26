---
title: "NaryEquationNode.LimitLocation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad NaryEquationNode. Este atributo especifica la ubicación de los límites en operadores nary. Los límites pueden estar centrados arriba y abajo del operador nary o posicionados justo a la derecha del operador"
type: docs
url: /es/net/aspose.cells.drawing.equations/naryequationnode/limitlocation/
---
## NaryEquationNode.LimitLocation property

Este atributo especifica la ubicación de los límites en operadores n-arios. Los límites pueden estar centrados arriba y abajo del operador n-ario, o posicionados justo a la derecha del operador.

```csharp
public EquationLimitLocationType LimitLocation { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyLimitLocationDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma para contener la ecuación
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // Accede a la ecuación y agrega un nodo de operador n-ario
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // Convertir a NaryEquationNode para acceder a LimitLocation
            var naryEquationNode = (NaryEquationNode)naryNode;

            try
            {
                // Mostrar LimitLocation actual (valor predeterminado)
                Console.WriteLine("Default LimitLocation: " + naryEquationNode.LimitLocation);

                // Establecer LimitLocation a SubSup (límites en el lado derecho)
                naryEquationNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("After setting to SubSup: " + naryEquationNode.LimitLocation);

                // Cambiar de nuevo a UndOvr (límites centrados)
                naryEquationNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("After setting to UndOvr: " + naryEquationNode.LimitLocation);

                // Guarda el libro de trabajo
                workbook.Save("LimitLocationDemo.xlsx");
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

* enum [EquationLimitLocationType](../../equationlimitlocationtype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



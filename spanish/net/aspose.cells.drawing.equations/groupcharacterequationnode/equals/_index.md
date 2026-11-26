---
title: "GroupCharacterEquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GroupCharacterEquationNode. Determinar si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/groupcharacterequationnode/equals/
---
## GroupCharacterEquationNode.Equals method

Determinar si el nodo de ecuación actual es igual al nodo especificado

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | El nodo especificado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class GroupCharacterEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear dos instancias de GroupCharacterEquationNode para comparar
            // Dado que GroupCharacterEquationNode no tiene un constructor sin parámetros,
            // necesitaremos crearlos a través de la ShapeCollection de la hoja de cálculo
            var shape1 = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var node1 = (GroupCharacterEquationNode)shape1.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            node1.GroupChr = "⏟";
            node1.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
            node1.Position = EquationCharacterPositionType.Bottom;
            node1.VertJc = EquationCharacterPositionType.Bottom;

            var shape2 = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var node2 = (GroupCharacterEquationNode)shape2.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            node2.GroupChr = "⏟";
            node2.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
            node2.Position = EquationCharacterPositionType.Bottom;
            node2.VertJc = EquationCharacterPositionType.Bottom;

            try
            {
                // Llamar al método Equals con el parámetro Object
                bool areEqual = node1.Equals((Object)node2);

                // Mostrar el resultado de la comparación
                Console.WriteLine($"The two GroupCharacterEquationNode instances are equal: {areEqual}");

                // Agregar el resultado a la hoja de cálculo
                worksheet.Cells["A1"].PutValue("GroupCharacterEquationNode Equals Comparison Result:");
                worksheet.Cells["A2"].PutValue(areEqual);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("GroupCharacterEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



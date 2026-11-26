---
title: "GroupCharacterEquationNode.GroupChr"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GroupCharacterEquationNode. Especifica un símbolo predeterminado U23DF. Se recomienda encarecidamente usar el atributo ChrType para establecer el carácter de acento. Utilice esta configuración de propiedad si no puede encontrar el carácter que necesita en un tipo conocido."
type: docs
url: /es/net/aspose.cells.drawing.equations/groupcharacterequationnode/groupchr/
---
## GroupCharacterEquationNode.GroupChr property

Especifica un símbolo (predeterminado U+23DF). Se recomienda encarecidamente usar el atributo ChrType para establecer el carácter de acento. Utilice esta configuración de propiedad si no puede encontrar el carácter que necesita en un tipo conocido.

```csharp
public string GroupChr { get; set; }
```

### Observaciones

Debe notarse que esta propiedad solo acepta un carácter, y si se pasan varios caracteres, solo se acepta el primer carácter.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class GroupCharacterEquationNodePropertyGroupChrDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una ecuación a la primera hoja de cálculo
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Obtener el nodo raíz de la ecuación
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Crear un nodo de carácter de grupo con doble flecha hacia la derecha
            GroupCharacterEquationNode groupNode = 
                (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Agregar texto base al carácter de grupo
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = 
                (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "abc";

            // Demostrar el uso de la propiedad GroupChr
            Console.WriteLine("Group Character: " + groupNode.GroupChr); // Should output "⇒"

            // Guarda el libro de trabajo
            workbook.Save("GroupCharacterEquationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



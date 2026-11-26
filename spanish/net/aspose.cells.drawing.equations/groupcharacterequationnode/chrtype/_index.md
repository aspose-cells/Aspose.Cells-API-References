---
title: "GroupCharacterEquationNode.ChrType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GroupCharacterEquationNode. Especificar caracteres combinados por valor de tipo."
type: docs
url: /es/net/aspose.cells.drawing.equations/groupcharacterequationnode/chrtype/
---
## GroupCharacterEquationNode.ChrType property

Especificar caracteres combinantes por valor de tipo.

```csharp
public EquationCombiningCharacterType ChrType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class GroupCharacterEquationNodePropertyChrTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una ecuación a la primera hoja de cálculo
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtener el nodo raíz de la ecuación
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Agregar un nodo de carácter de grupo
            GroupCharacterEquationNode groupNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            
            // Establecer propiedades del carácter de grupo
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Agregar texto base
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "test";

            // Guarda el libro de trabajo
            workbook.Save("GroupCharacterEquationDemo.xlsx");

            // Verifique el archivo guardado
            Workbook verifyWorkbook = new Workbook("GroupCharacterEquationDemo.xlsx");
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            GroupCharacterEquationNode verifyNode = (GroupCharacterEquationNode)verifyTextBox.GetEquationParagraph()
                .GetChild(0).GetChild(0);

            Console.WriteLine("Group Character Type: " + verifyNode.ChrType);
            Console.WriteLine("Group Character: " + verifyNode.GroupChr);
            Console.WriteLine("Base Text: " + ((TextRunEquationNode)verifyNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### Ver también

* enum [EquationCombiningCharacterType](../../equationcombiningcharactertype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


